# Baselines_UR5_issue
Openai_baselines_UR5_DRL_training Issue with attribute error as description in below.<br>

2019-01-24 10:21:38.551305: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2 FMA
Creating a DDPG agent with action space 4 x [0.15       0.05       0.26179939 0.26179939]...
Traceback (most recent call last):
  File "/home/huong/catkin_ws/src/ur_gazebo_test2/experiment/train.py", line 224, in <module>
    main()
  File "/home/huong/env_tensorflow/lib/python3.5/site-packages/click/core.py", line 764, in __call__
    return self.main(*args, **kwargs)
  File "/home/huong/env_tensorflow/lib/python3.5/site-packages/click/core.py", line 717, in main
[INFO] [1548292899.141068, 877.931000]: DONE CONFIGURE DDPG
    rv = self.invoke(ctx)
  File "/home/huong/env_tensorflow/lib/python3.5/site-packages/click/core.py", line 956, in invoke
    return ctx.invoke(self.callback, **ctx.params)
  File "/home/huong/env_tensorflow/lib/python3.5/site-packages/click/core.py", line 555, in invoke
    return callback(*args, **kwargs)
  File "/home/huong/catkin_ws/src/ur_gazebo_test2/experiment/train.py", line 220, in main
    launch(**kwargs)
  File "/home/huong/catkin_ws/src/ur_gazebo_test2/experiment/train.py", line 194, in launch
    rollout_worker = RolloutWorker(params['make_env'], policy, dims, logger, **rollout_params)
  File "/home/huong/baselines/baselines/her/util.py", line 36, in wrapper
    return method(*positional_args, **keyword_args)
  File "/home/huong/baselines/baselines/her/rollout.py", line 42, in __init__
    self.reset_all_rollouts()
  File "/home/huong/baselines/baselines/her/rollout.py", line 46, in reset_all_rollouts
    self.obs_dict = self.venv.reset()
AttributeError: 'function' object has no attribute 'reset'

Process finished with exit code 1

