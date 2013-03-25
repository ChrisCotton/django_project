# django_project

## Sample Django Project to Hammer out github workflow

*single asterisks*

_single underscores_

**double asterisks**

__double underscores__

### Some basic Markdown syntax stuff ( from the docs )

***

I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"



Visit [Daring Fireball][] for more information.
[Daring Fireball]: http://daringfireball.net/ 

### How we propose to push public branches ( Non local & accesssable by anyone )

> * $ git clone git://github.com/mettadore/tutorials.git
> * $ cd tutorials
> * $ git branch
> * \* master
> * $ git checkout -b public
> > Switched to a new branch 'public'
> * $ echo "Some random change"&gt; README
> * $ git commit -a -m "Update readme"
> * $ git push origin public
> * $ git branch
> * \* master
> * public
> * $

***


### How we merge private branches back into master. and then keep working on local copy: 

> 1. $ git checkout -b topic
> > Work a bit and commit changes
> 2. $ git pull origin master
> 3. $ git rebase master
> > Work a bit and commit changes
> 4. $ git pull origin master
> 5. $ git rebase master
> > Work a bit and commit changes
> > When you're ready to make everything official:
> 6. $ git checkout master
> 7. $ git merge topic
> 8. $ git push
> 9. $ git branch -D topic  ##### or, as I do, keep using the local branch for more changes
>> Getting closer to what I want. 
 


