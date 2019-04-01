# FritzAhaClient
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fwolpl%2FFritzAhaClient.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fwolpl%2FFritzAhaClient?ref=badge_shield)

[![](https://jitpack.io/v/wolpl/FritzAhaClient.svg)](https://jitpack.io/#wolpl/FritzAhaClient)


A Kotlin/JVM client for accessing the AVM Fritzbox AHA-HTTP Interface.
## Usage in your gradle project
### 1. Include dependency
``` gradle
allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
} 
```
``` gradle
dependencies {
    implementation 'com.github.wolpl:FritzAhaClient:Tag'
}
```
### 2. Use a FritzSession
````kotlin
fun main(){
    val session = FritzSession("username", "password")
    val switches = session.getSwitchList()
    println("Available switches: $switches")
}
````


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fwolpl%2FFritzAhaClient.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fwolpl%2FFritzAhaClient?ref=badge_large)