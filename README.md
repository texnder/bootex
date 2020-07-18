# bootex

v1.0.9
========

## Call non-static method as static method

bluff::class added to call non-static function in static way. this class is similar to laravel facade::class

## Middelware

Middelware is the root class for all middelware classes. can be included using bluff::class

Middelwares will be call before respones genration. to use this functionality user must have [routex](https://github.com/texnder/routex) (>=v1.0.6) 


v 1.0.3
=========

namespace container for bootstrap service integration

## scan directories to add 

add packages directory path and their respective namespaces into [psr4.php] file.

bootex services class uses psr4 namespacing convention to scan and generate full namespace for available [php] files in given directories and their subdirectories recursively.

## bootex services class also accepts file path as an argument

if project developer do not want to manage bootex [psr4.php] file then, there is no problem, developer can manage it from anywhere. they only have to do is, while creating bootex [services] class instance pass an argument of absolute path of the file which returns array, In which, psr4 sets as key of array and its value is an array of packages directories with their respected namespace, similar to bootex [psr4.php] file, to scan and add files namespaces in bootex/services object.

## Documentation

documentation for all texnder APIs available [here](http://texnder.com/documentation/)

## License

The bootex is open-sourced php library licensed under the [MIT license](http://opensource.org/licenses/MIT).
