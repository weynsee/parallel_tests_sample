Run the specs through parallel_rspec and it returns 1 pending only:
  
  `parallel_rspec spec/`

```
2 processes for 1 specs, ~ 0 specs per process
*

Pending:
  test tests something
    # no tests
    # ./spec/test_spec.rb:2

Finished in 0.00048 seconds
1 example, 0 failures, 1 pending

1 example, 0 failures, 1 pending

Took 1.365892 seconds
```

Run the specs through guard and the number doubles.
```
[1] guard(main)>
00:34:56 - INFO - Run all
00:34:56 - INFO - Running all specs
2 processes for 1 specs, ~ 0 specs per process
*

Pending:
  test tests something
    # no tests
    # ./spec/test_spec.rb:2

Finished in 0.00048 seconds
1 example, 0 failures, 1 pending


2 examples, 0 failures, 2 pendings

Took 1.667804 seconds
```
