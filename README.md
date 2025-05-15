# moodle-brackets-test

Just testing if escaping double curly brackets works to escape mustache tags on Moodle.

```jsx
export function UserProvider({ children }) {
  return (
    <UserContext.Provider value=&#123;&#123; username: "bob" &#125;&#125;>
      {children}
    </UserContext.Provider>
  );
}
```
