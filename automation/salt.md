# SALT
---

### Running salt apply

```bash
salt '*' state.apply test=True
```

#### Arguments


```
test				Run states in test-only (dry-run) mode
mock				state run to execute without actually calling any states
exclude				Exclude specific states from execution					
```
