# change file stat

# check file stat
using `File.stat`, return a file state object, examples:
```ruby
s = File.stat('filename');
File.chmod(s.mode,'newfilename')
```

# open file with specific stat
```ruby
s = File.stat('filea')
fh = File.new('filename','w',s.mode)
```