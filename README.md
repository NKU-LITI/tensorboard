
- tensorboard/qwen25_math7b_2555ocaf_grpo_baseline_in_luffy

在 luffy verl0.1.0 实现的grpo，参数配置如下:

```
algorithm.grpo_use_std=False \
actor_rollout_ref.actor.loss_remove_token_mean=True \
```


- tensorboard/qwen25_math7b_grpo_openr1_in_srft

在 srft verl0.1.0 上，使用25000+数据集 实现的 grpo


- qwen25_math7b_grpo_all_agg_adapt_npu：在gpu verl0.7.0上实现的grpo，entropy_loss和pg_loss都使用tokenmean (agg_loss)，目的是check npu和gpu性能是否有差别