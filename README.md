# 3 Principais formas de renderizações no React

## Pai para filho
```tsx
  <Pai>
    <Filho />
  </Pai>
```

## Propriedade
```tsx
  <Pai>
    <Filho title="" />
  </Pai>
```

## Hooks (useState, useContext, useReducer)
```tsx
  function Component() {
    const [state, setState] = useState();
  }
```


# Fluxo de renderização

1. Gerar uma nova versão do componente que precisa ser renderizado;
2. Comparar essa nova versão com a versão anterior já salva na página;
3. Se houverem alterações, o React "Renderiza" essa nova versão em tela; (Reconciliation)
