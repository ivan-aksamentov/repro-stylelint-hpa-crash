# repro-stylelint-hpa-crash

Reproduces a crash in [kristerkari/stylelint-high-performance-animation](https://github.com/kristerkari/stylelint-high-performance-animation) on the following CSS fragment:

```css
:root {
  --sidebar-transition: all 0.3s ease;
}

.example {
  transition: var(--sidebar-transition);
}

```

## How to reproduce
```bash
git clone https://github.com/ivan-aksamentov/repro-stylelint-hpa-crash
yarn install
stylelint crash.css

```

## License
MIT
