# FLDRL-in-Wireless-Communication
Apply  Deep Reinforcement Learning aided by Federated Learning to Wireless Comunication
## Enhanced Multi Acess using Deep Reinforcement Learning aided by Federated Learning

### Apply Deep RL into FL
#### Solution: Using [Pysyft](<https://github.com/OpenMined/PySyft>)

- PySyft is a Python library for secure and private Deep Learning.
- PySyft decouples private data from model training, using [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Multi-Party Computation (MPC)](https://en.wikipedia.org/wiki/Secure_multi-party_computation) within the main Deep Learning frameworks like PyTorch and TensorFlow.
- [Tutorial](<https://github.com/OpenMined/PySyft/tree/master/examples/tutorials>) provides a set of examples on applying RL into FL.



#### Reinforcement Learning with Model Allocation

---

###### Notes

- In `config.py`, we only load model but not save model.

  - ```
    self.saveModel = False
    self.loadModel = True
    ```

- Run `python3 test_CSMA_DQN_withModelAllocation.py` to proceed training.

- `Throughput` is about `5.2`-`5.4`

###### Training log

| Number of Station | Max Avg Throughput | Total training epoch |
| ----------------- | ------------------ | -------------------- |
| 5                 | 5.45               | 10w                  |
| 10                | 5.46               | 13w                  |
| 20                | 5.28               | 22w                  |

