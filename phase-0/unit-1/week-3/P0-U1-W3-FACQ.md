## Using Ruby `reduce` to combine an array

`reduce` is a useful method to use when doing challenges. The method takes elements inside of an array and combines them as you wish.

If I wanted to add up all the numbers in this array `[1, 2, 3, 4, 5]`, I could just run:
```ruby
  [1, 2, 3, 4, 5].reduce(:+)
  # Returns  => 15
```

This is simply saying  `+` all the elements in the array together. The shorthand `:+` is just one of those things you have to get used to.


Let's use it to multiply all the elements in an array.

```ruby
  [1, 2, 3, 4, 5].reduce(:*)
  # Returns  => 120
```

You can also use reduce on ranges

```ruby
  (1..5).reduce(:*)
  # Returns  => 120
  
  (1..5).reduce(:+)
  # Returns  => 15
```

[Here are the Ruby docs on reduce](http://ruby-doc.org/core-2.2.1/Enumerable.html#method-i-reduce)

## Using Ruby `inject` to compare elements in an array

When working through the problem of trying to find the longest word in an array, we found the `inject` method to do the job nicely.

`inject` will run each element of an array through whatever comparison you want.

The below example uses the `currentchamp` and `upnext` variables to better visualize what reduce is doing. The first element in the array automatically becomes `currentchamp` by default. But then it is compared to `upnext`. 

Whichever string is longer will become `currentchamp`. Then, `inject` repeats this process *until all elements in the array have been compared*.

```ruby
def longest_string(string_arr) # find the longest word
  string_arr.inject do |currentchamp, upnext|
    if currentchamp.length > upnext.length
      currentchamp
    else
      upnext
    end
#   currentchamp.length > upnext.length ? currentchamp : upnext
  end
end
puts longest_string(["Bob", "Teddy", "Kennedy"])
```

The version using the ternary operator (shorthand for if/else) is much shorter, but less readable to me.

```ruby
def longest_string(string_arr) # find the longest word
  string_arr.inject do |currentchamp, upnext|
    currentchamp.length > upnext.length ? currentchamp : upnext
  end
end
puts longest_string(["Bob", "Teddy", "Kennedy"])
```

[Here's the Ruby docs on inject](http://ruby-doc.org/core-2.2.1/Enumerable.html#method-i-inject)
