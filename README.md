# Docs
[http://getinstance.info/articles/react/learning-react-redux/](http://getinstance.info/articles/react/learning-react-redux/)

[https://rajdee.gitbooks.io/redux-in-russian/content/](https://rajdee.gitbooks.io/redux-in-russian/content/)

[https://www.tutorialspoint.com/reactjs/reactjs_using_flux.htm](https://www.tutorialspoint.com/reactjs/reactjs_using_flux.htm)

[https://facebook.github.io/react/docs/forms.html](https://facebook.github.io/react/docs/forms.html)

[http://stackoverflow.com/questions/1129216/sort-array-of-objects-by-string-property-value-in-javascript](http://stackoverflow.com/questions/1129216/sort-array-of-objects-by-string-property-value-in-javascript)

[https://maxfarseer.gitbooks.io/redux-course-ru/content/combinereducers.html](https://maxfarseer.gitbooks.io/redux-course-ru/content/combinereducers.html)

[https://jquense.github.io/react-widgets/docs/#/getting-started?_k=4yyzja](https://jquense.github.io/react-widgets/docs/#/getting-started?_k=4yyzja)

[https://github.com/reactjs/react-modal](https://github.com/reactjs/react-modal)

[https://github.com/recharts/recharts](https://github.com/recharts/recharts)

[https://flow.org/](https://flow.org/)

[https://facebook.github.io/immutable-js/](https://facebook.github.io/immutable-js/)

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
 
git config --global user.name "username"
git config --global user.email “email”

prepareMultipleSort(prop: string, sort: string) {
        return (obj1: Array<Object>, obj2: Array<Object>): number => {
            return obj1[prop] > obj2[prop] ? (sort === "ASC" ? 1 : -1) :
                obj1[prop] < obj2[prop] ? (sort === "ASC" ? -1 : 1) : 0;
        };
    }

    doMultipleSort(cols: Array<string>, sort: string) {
        return (obj1: Array<Object>, obj2: Array<Object>) => {
            let result = 0;

            for (let col of cols) {
                result = (result === 0) && this.prepareMultipleSort(col, sort)(obj1, obj2);
            }

            return result;
        };
    }

        //sort by state then deal_id before output
        data.sort(this.doMultipleSort(["state", "deal_id"], "DESC"));

