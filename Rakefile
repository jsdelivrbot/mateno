task :scale, [:size] do |t, args|
  `heroku ps:scale worker=#{args[:size]}`
end

task :deploy, [:message] do |t, args|
  `git add -A`
  `git commit -m "#{args[:message]}"`
  `git push origin master`
end
