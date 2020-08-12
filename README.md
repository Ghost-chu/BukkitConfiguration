# BukkitConfiguration
This is a **Unofficial** cross-platform Bukkit YamlConfiguration implement.

## Issues / Feedback
https://github.com/Ghost-chu/BukkitConfiguration/issues

## Read YAML File
First, Add this to your dependency.
Second, 
```JAVA
FileConfiguration fileConfiguration = YamlConfiguration.loadConfiguration(new File("test.yml"));
fileConfiguration.getString("path.to.str");
fileConfiguration.getBoolean("path.to.boolean");
fileConfiguration.set("apple-color", "red");
fileConfiguration.set("friends.alex.age", 18);
fileConfiguration.set("useless-field", null); //Set to null to delete.
ConfigurationSection section = fileConfiguration.getConfigurationSection("friends");
section.getInt("alex.age");
List<String> strList = fileConfiguration.getStringList("meme");
```
And more! Enjoy!

## Upstream 
https://hub.spigotmc.org/stash/projects/SPIGOT/repos/bukkit/browse

## Maven repo
```XAML
<repository>
    <id>quickshop-repo</id>
    <url>https://repo.codemc.io/</url>
</repository>

<dependency>
    <groupId>cc.bukkit</groupId>
    <artifactId>BukkitConfiguration</artifactId>
    <version>1.16.1-R0.1-SNAPSHOT</version>
</dependency>
```
