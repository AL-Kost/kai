<p align="center">
  <img src="utils/kai.png" alt="Application Logo" width="300">
</p>
Load balancer for GPU nodes designed to optimally assign LLM inference tasks.

# Goals & Features

* Easily add/remove nodes, update hardware info.
* Easily add new type of tasks, store required hardware and be able to update it on-the-fly.
* Logging to PostgreSQL.
* Easily schedule node and block all other assignments of it. Be able to unblock node after assignment processing.
* Custom logic of balancer. (All GPU nodes are not equal - from RTX3090 to A100. Also, all tasks require not equal amount of resources. For example, Summarization = 24GB VRAM, NER=8GB VRAM)

