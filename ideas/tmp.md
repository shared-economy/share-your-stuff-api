# Temp Ideas

MongoDB:
- create a collection based on user uuid
- create a collection based on object uuid
- create a collection based on group uuid

Store in the following order:
```
Group(UserRef,UserRef,Object,Object,Object)
```
The concept is that each group owns each object and has references to the user which is part of the group.

In contrast the user setup includes the only a reference to the objects

User(ObjectRef,ObjectRef)

```js
DB_user{User1{UUID1, firstname, lastname, ...},User2{UUID2, ...}}
DB_object(UUID)
```
