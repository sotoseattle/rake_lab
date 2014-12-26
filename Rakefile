require 'rake'

desc 'Open tmux environment for sotoseattle blog'
task :blog do |t|
  cd '/Users/fjs6/work/renewal/sotoseattle'
  sh "tmux new-session -s blog -n edit -d"
  sh "tmux send-keys -t blog 'vim' C-m"
  sh "tmux new-window -n server -t blog"
  sh "tmux send-keys -t blog:2 'rake generate' C-m"
  sh "tmux send-keys -t blog:2 'rake preview' C-m"
  sh "tmux new-window -n shell -t blog"
  sh "tmux send-keys -t blog:3 'ls -t source/_posts/* | head -10' C-m"
  sh "tmux select-window -t blog:1"
  sh "tmux attach -t blog"
end
