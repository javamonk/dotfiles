require 'rake'

# Files to be excluded from the install
@non_dotfiles = FileList["README.md", "Rakefile", "backup", ".", "..",]

desc "Backups dotfiles in backup directory"
task :backup do
  puts "Backing up rake files"
 
  # dot files to be installed 
  dotfiles = Dir.glob('**', File::FNM_DOTMATCH) - @non_dotfiles
  puts dotfiles

  # dot files to be backed up
  for dotfile in dotfiles do
    puts "Looking for #{dotfile} to backup"
    # Check if the file exists in your home directory

  end

  puts `$HOME`
end

desc "Installs the dot files by creating the various symlinks"
task :install => [:backup] do
  
  puts "Installing"
end

desc "Removes and dot file symlinks and returns the backed up dot files"
task :uninstall do
  puts "Uninstalling"
end

task :default => 'install'
