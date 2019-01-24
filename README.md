# Baselines_UR5_issue
Openai_baselines_UR5_DRL_training Issue with attribute error as description in below.<br>

2019-01-24 10:21:38.551305: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2 FMA<br>
Creating a DDPG agent with action space 4 x [0.15       0.05       0.26179939 0.26179939]...<br>
Traceback (most recent call last):<br>
  File "/home/huong/catkin_ws/src/ur_gazebo_test2/experiment/train.py", line 224, in <module><br>
    main()<br>
  File "/home/huong/env_tensorflow/lib/python3.5/site-packages/click/core.py", line 764, in __call__<br>
    return self.main(*args, **kwargs)<br>
  File "/home/huong/env_tensorflow/lib/python3.5/site-packages/click/core.py", line 717, in main<br>
[INFO] [1548292899.141068, 877.931000]: DONE CONFIGURE DDPG<br>
    rv = self.invoke(ctx)<br>
  File "/home/huong/env_tensorflow/lib/python3.5/site-packages/click/core.py", line 956, in invoke<br>
    return ctx.invoke(self.callback, **ctx.params)<br>
  File "/home/huong/env_tensorflow/lib/python3.5/site-packages/click/core.py", line 555, in invoke<br>
    return callback(*args, **kwargs)<br>
  File "/home/huong/catkin_ws/src/ur_gazebo_test2/experiment/train.py", line 220, in main<br>
    launch(**kwargs)<br>
  File "/home/huong/catkin_ws/src/ur_gazebo_test2/experiment/train.py", line 194, in launch<br>
    rollout_worker = RolloutWorker(params['make_env'], policy, dims, logger, **rollout_params)<br>
  File "/home/huong/baselines/baselines/her/util.py", line 36, in wrapper<br>
    return method(*positional_args, **keyword_args)<br>
  File "/home/huong/baselines/baselines/her/rollout.py", line 42, in __init__<br>
    self.reset_all_rollouts()<br>
  File "/home/huong/baselines/baselines/her/rollout.py", line 46, in reset_all_rollouts<br>
    self.obs_dict = self.venv.reset()<br>
AttributeError: 'function' object has no attribute 'reset'<br>
<br>
Process finished with exit code 1<br>

