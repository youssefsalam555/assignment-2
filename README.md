# assignment-2
youssef sheref-20201047
# Train and save the model with the optimal total_timesteps
model = DQN("MlpPolicy", env, learning_rate=1e-3, verbose=0)
model.learn(total_timesteps=optimal_timesteps)

# Save the model
model.save("optimal_dqn_taxi")
