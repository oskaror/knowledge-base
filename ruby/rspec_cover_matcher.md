You can use the cover matcher to specify that a range covers one or more
expected objects. This works on any object that responds to #cover?
(such as a Range):

```ruby
  expect(1..10).to cover(5)
  expect(1..10).to cover(4, 6)
  expect(1..10).not_to cover(11)
```
[RSpec documentation](https://relishapp.com/rspec/rspec-expectations/v/3-9/docs/built-in-matchers/cover-matcher)