一个简单的守护进程

<pre><code>
package main

import (
  "github.com/dale-di/daemon"
)

func main() {
  dmfiles := []string{}
  //dmfiles := []string{"", "/tmp/mydaemon.out", "/tmp/mydaemon.err"}
  daemon.Daemon("/tmp/mydaemon.pid", dmfiles, "")
  ....
}
</code></pre>
