# Docs
[http://getinstance.info/articles/react/learning-react-redux/](http://getinstance.info/articles/react/learning-react-redux/)

[https://rajdee.gitbooks.io/redux-in-russian/content/](https://rajdee.gitbooks.io/redux-in-russian/content/)

[https://www.tutorialspoint.com/reactjs/reactjs_using_flux.htm](https://www.tutorialspoint.com/reactjs/reactjs_using_flux.htm)

[https://facebook.github.io/react/docs/forms.html](https://facebook.github.io/react/docs/forms.html)

[http://stackoverflow.com/questions/1129216/sort-array-of-objects-by-string-property-value-in-javascript](http://stackoverflow.com/questions/1129216/sort-array-of-objects-by-string-property-value-in-javascript)

[https://maxfarseer.gitbooks.io/redux-course-ru/content/combinereducers.html](https://maxfarseer.gitbooks.io/redux-course-ru/content/combinereducers.html)

# Commands

### ssh
ssh-add -L - view ssh key

### git
git remote rm origin
git remote add origin git@github.com:org/rep.git

git config --global color.branch auto
git config --global color.diff auto
git config --global color.interactive auto
git config --global color.status auto
 
git config --global alias.nmerge "merge --no-ff"
git config --global alias.co "checkout"
git config --global alias.br "branch"
git config --global alias.ci "commit"
git config --global alias.st "status"
git config --global alias.unstage "reset --hard HEAD^"
git config --global alias.last "log -1 HEAD"
git config --global alias.lg "log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative"
 
git config --global user.name "romkacrv"
git config --global user.email “silveriddqd@gmail.com”


### vpn
sudo bash
apt-get install openvpn
cp Adyax_rchernov_gw.adyax.com.ovpn /etc/openvpn/
mv /etc/openvpn/Adyax_rchernov_gw.adyax.com.ovpn /etc/openvpn/openvpn.conf
apt-get install traceroute
/etc/init.d/openvpn start
ping 8.8.8.8
update-rc.d -f openvpn remove

/etc/init.d/openvpn start
/etc/init.d/openvpn stop

