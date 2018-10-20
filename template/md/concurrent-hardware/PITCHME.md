### Concurrent Hardware API

This API returns the number of logical processors available to run threads on the user's device.

Note:

Modern computers have multiple physical processor cores in their CPU (two or four cores is typical), but each physical core is also usually able to run more than one thread at a time using advanced scheduling techniques. So a four-core CPU may offer eight logical processor cores, for example. The number of logical processor cores can be used to measure the number of threads which can effectively be run at once without them having to context switch.
