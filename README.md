# setlock.rb
`setlock.rb` is a Ruby port of `setlock` in [daemontools].

The purpose of this program is to provide functionality of `setlock` without installing [daemontools].

[daemontools]: https://cr.yp.to/daemontools.html

# Usage
```
Usage: setlock.rb [ -nNxX ] file program [ arg ... ]
    -n  No delay. If fn is locked by another process, setlock gives up.
    -N  (Default.) Delay. If fn is locked by another process, setlock waits until it can obtain a new lock.
    -x  If fn cannot be opened (or created) or locked, setlock exits zero.
    -X  (Default.) If fn cannot be opened (or created) or locked, setlock prints an error message and exits nonzero.
```
