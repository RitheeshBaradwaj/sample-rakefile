require 'fileutils'

desc 'executing a script'
task :run_command do
    sh "powershell.exe ./script.ps1" do |ok, res|
        if ! ok
            puts "Something went wrong (status = #{res.exitstatus})"
        end
    end
end

desc "default task"
task :default => ["run_command"]
