#### UserSample.java

```java
package jp.kronos.sample;

import java.util.ArrayList;
import java.util.List;

import jp.kronos.dto.User;

public class UserSample {
    List<User> users = new ArrayList<>();
    
    public UserSample() {
        User user1 = new User("user01", "pass01", "Yamada", "Taro");
        User user2 = new User("user02", "pass02", "Suzuki", "Hanako");
        User user3 = new User("user03", "pass03", "Tanaka", "Gonzalez");
        
        users.add(user1);
        users.add(user2);
        users.add(user3);
    }
    
    public void showUsers() {
        for (User user : users) {
            System.out.println(user.getLastName() + " " + user.getFirstName());
        }
    }
    
    public boolean login(String loginId, String password) {
        for (User user : users) {
            if (user.getLoginId().equals(loginId) && user.getPassword().equals(password)) {
                return true;
            }
        }
        return false;
    }
}
```

#### ApiMain19.java

```java
package jp.kronos.main;

import jp.kronos.sample.UserSample;

public class ApiMain18 {

    public static void main(String[] args) {
        UserSample userSample = new UserSample();
        
        if (userSample.login("user01", "pass02")) {
            System.out.println("Login Success!");
        } else {
            System.out.println("Login Failure!");
        }
    }

}
```
