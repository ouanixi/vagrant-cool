# Vagrant Box for Cool

Set up the development environment for [Cool: The Classroom Object-Oriented Language](http://theory.stanford.edu/~aiken/software/cool/cool.html) using [Vagrant](https://www.vagrantup.com/).

## Usage

This is a fairly simple project to get up and running.

1. Clone the project
2. Make sure [vagrant](https://www.vagrantup.com/downloads.html) is installed
3. Run `vagrant up`
4. Use the folder `cs143` in this repo to store your files. They will be mapped to the VM folder ~/cs143 from which you can compile and run your files.
5. Connect to the virtual machine and test using `vagrant ssh`. You will see your `cs143` in there.
6. Compile and run your code from within the VM.



## Reference

- [Stanford Compilers Course on edx](https://www.coursera.org/course/compilers)

## License

vagrant-cool is available under the MIT license. See the LICENSE file for more info.

## Credit
[dlackty](https://github.com/dlackty/vagrant-cool). I took their project and tweaked it to work with edx version.