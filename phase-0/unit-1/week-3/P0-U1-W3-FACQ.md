## Using `reduce` to get a result

`reduce` is a useful method to use when doing challenges. The method takes elements inside of an array and combines them as you wish.

If I wanted to add up all the numbers in this array `[1, 2, 3, 4, 5]`, I could just run:
```ruby
  [1, 2, 3, 4, 5].reduce(:+)
  # Returns  => 15
```

This is simply saying take the array and `+` all the elements together. The shorthand `:+` is just one of those things you have to get used to.


So let's use it to multiply all the elements in an array.

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
