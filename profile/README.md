[![State-of-the-art Shitcode](https://img.shields.io/static/v1?label=State-of-the-art&message=Shitcode&color=7B5804)](https://github.com/trekhleb/state-of-the-art-shitcode)
```java
for (String q : QueuePlugin.getInstance().getQueuesFile().getConfigurationSection("queues").getKeys(false)) {
    ConfigurationSection section = QueuePlugin.getInstance().getQueuesFile().getConfigurationSection("queues." + q);

    Queue queue = new Queue(q);
    queue.setRequiredNiggers(section.getInt("requiredPlayers"));
    queue.setTargetServer(section.getString("bungeecord"));

    queues.add(queue);
}
```
