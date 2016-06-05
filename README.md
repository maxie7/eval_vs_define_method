### 'eval' or 'define_method'

We'll benchmark the performance of methods created by define_method and those created through eval.

* As we can see from the results (run & see eval_vs_define_method.rb), the methods defined using eval() performed better than those created using define_method.

* But 'eval' itself performs poorly though methods created with it are quick. This is worth noting, because if you need to create a lot of new methods at runtime (a very rare scenario), 'define_method' is the better option. See 'dont_use_eval.rb' that demonstrates the relative performance of creating lots of new methods using eval versus define_method.
