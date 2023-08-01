<div id="top"></div>
<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>

Requirements
General
Allowed editors: vi, vim, emacs
All your files will be interpreted on Ubuntu 20.04 LTS
All your files should end with a new line
A README.md file, at the root of the folder of the project, is mandatory
All your Bash script files must be executable
The first line of all your Bash scripts should be exactly #!/usr/bin/env ruby
All your regex must be built for the Oniguruma library

<p align="right">(<a href="#top">back to top</a>)</p>
<p align="right">(<a href="#readme-top">back to top</a>)</p>

Background Context
For this project, you have to build your regular expression using Oniguruma,
a regular expression library that which is used by Ruby by default. Note that
other regular expression libraries sometimes have different properties.

Because the focus of this exercise is to play with regular expressions (regex),
here is the Ruby code that you should use, just replace the regexp part,
meaning the code in between the //:

sylvain@ubuntu$ cat example.rb
#!/usr/bin/env ruby
puts ARGV[0].scan(/127.0.0.[0-9]/).join
sylvain@ubuntu$
sylvain@ubuntu$ ./example.rb 127.0.0.2
127.0.0.2
sylvain@ubuntu$ ./example.rb 127.0.0.1
127.0.0.1
sylvain@ubuntu$ ./example.rb 127.0.0.a

<p align="right">(<a href="#top">back to top</a>)</p>
<p align="right">(<a href="#readme-top">back to top</a>)</p>
