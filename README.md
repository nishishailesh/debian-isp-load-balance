# debian-isp-load-balance
## Install Net-ISP-Balance
```git pull https://github.com/lstein/Net-ISP-Balance```\
```perl ./Build.PL```\
It may give error because Module::Build is not installed\
```cpan Module::Build```\
It may give error because  ```make``` is not installed\
```apt install make```\
```cpan Module::Build```\
```perl ./Build.PL```\
a script named "Build" is added in installation folder
```perl Build installdeps```\
