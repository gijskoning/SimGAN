**main_gail_dyn_ppo** is used to train the simulator with the behaviour policy
**main** is used to refine the policy on the tuned simulator

### For hopper deform training:
Both work with environment: HopperCombinedEnv-v1 which is in file hopper_env_combined_policy.py with class HopperCombinedEnv
The environment uses a PPO algorithm as well. Which is saved here: rained_models_Gdyn_hopper_bullet_deform_new11_comb_f${id}/ppo

--use-split-pi is only used when training the simulator. With the argument the SplitPolicy is used in main_gail_dyn_ppo.py

The actor_critic arguments used in code refer to either Policy or SplitPolicy defined in a2c_ppo_acktr/model...