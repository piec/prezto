A modified version of prezto which adds bundle support. Bundles are prezto modules that live outside of the prezto source tree. (Similar to [vim's vundle](https://github.com/gmarik/Vundle.vim))

This version adds a `bundle` command that is used to interract with bundles:
  ```
  # install a bundle from a github repository
  bundle install piec/powerline-prezto

  # load all bundles
  bundle load
  
  # update all bundles
  bundle update
  ```

zstyle ':prezto:module:bundle' modules \
  'piec/k-prezto'
  'piec/powerline-prezto'
```

The bundle mechanism is itself implemented as a simple [prezto module](https://github.com/piec/prezto/tree/bundle/modules/bundle)
