### jedis
---
https://github.com/xetorthio/jedis

```java
Jedis jedis = new Jedis("localhost");
jedis.set("foo", "bar");
String value = jedis.get("foo");

Set<HostAndPort> jedisClusterNodes = new HashSet<HostAndPort>();
jedisClusterNodes.add(new HostAndPort("127.0.0.1", 7379));
JedisCluster jc = new JedisCluster(jedisClusterNodes);
jc.set("foo", "bar");
String value = jc.get("foo");
```

```java
//

public class MigrateParams extends Params {
  
  private static final String COPY = "COPY";
  private static final String REPLACE = "REPLACE";
  private static final String AUTH = "AUTH";
  
  public MigrateParams() {
  }
  
  public static MigrateParams migrateParams() {
    return new MigratParams();
  }
  
  public MigrateParams copy() {
    addParams(COPY);
    return this;
  }
  
  public MigrateParams replace() {
    addParams(REPLACE);
    return this;
  }
  
  public MigrateParams auth(String password) {
    addParam(AUTH, password);
    return this;
  }
}
```

```
```


