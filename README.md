# moodle-brackets-test

Just testing if escaping double curly brackets works to escape mustache tags on Moodle.

## HTML Codes

This way doesn&apos;t work.

```jsx
export function UserProvider({ children }) {
  return (
    <UserContext.Provider value=&#123;&#123; username: "bob" &#125;&#125;>
      {children}
    </UserContext.Provider>
  );
}
```

## Other unicode characters (this may look silly)

Small curly brackets (U+FE5B, U+FE5C)

```jsx
export function UserProvider({ children }) {
  return (
    <UserContext.Provider value=﹛﹛ username: "bob" ﹜﹜>
      {children}
    </UserContext.Provider>
  );
}
```

Fullwidth curly brackets (U+FF5B, U+FF5D)

```jsx
export function UserProvider({ children }) {
  return (
    <UserContext.Provider value=｛｛username: "bob" ｝｝>
      {children}
    </UserContext.Provider>
  );
}
```
