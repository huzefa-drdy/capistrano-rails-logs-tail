namespace :rails do
  desc "Tail rails logs from server"
  task :logs do
    SSHKit.config.output_verbosity = Logger::DEBUG
    on roles(:app) do
      execute "tail -f #{current_path}/log/#{fetch(:rails_env)}.log"
    end
  end
end
