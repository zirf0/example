# SalesPlatform for OpenShift PaaS


SalesPlatform is a fork of VtigerCRM adapted for Russian Federation. Version 6.4.0
# Setup


1) <a href="https://www.openshift.com/app/account/new">Create</a> an account at https://www.openshift.com
2) Install git, ruby <a href=""https://developers.openshift.com/en/getting-started-overview.html>rhc</a> 
3) Create a php application with mysql:

    $ rhc app create spexample php-5.3 mysql-5.5 

4) Add this upstream repo

    $ cd spexample
    $ git remote add upstream -m master git://github.com/zirf0/example.git
    $ git pull -s recursive -X theirs upstream master

5) Then push the repo upstream

    $ git push

6) That's it, you can now checkout your application at:

    http://spexample-$yourdomain.rhcloud.com

7) Follow installatin procedure
