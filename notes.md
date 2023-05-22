bundle exec jekyll serve --host 0.0.0.0

recordar unir el branch master con feature, hay un cambio por empujar

"Adding notes to gitignore"

# Commands to do rsync file synchonization

- sudo rsync -anv /root/.bashrc wilder@159.223.105.208:/root/
- sudo rsync -anv /home/wilder/.vimrc wilder@159.223.105.208:/home/wilder/
- rsync -anv /home/wilder/.vimrc wilder@159.223.105.208:/home/wilder/
- rsync -av /home/wilder/.vimrc wilder@159.223.105.208:/home/wilder/
- rsync -anv ./_site/ wilder@159.223.105.208:/var/www/lafortunasc.info/html
- JEKYLL_ENV=production bundle exec jekyll build --config _config_prod.yml



# Steps to compile website
- Make sure push changes were already commited
- Remeber to use JEKYLL_ENV variable and set it to production to keep files synchronized
- Push to server with the command `JEKYLL_ENV=production bundle exec jekyll build --config _config_prod.yml`, and
remove the 'n' flag to push definitely(since the 'n' flag just run dry...)
- JEKYLL_ENV=production bundle exec jekyll build --config _config_prod.yml
