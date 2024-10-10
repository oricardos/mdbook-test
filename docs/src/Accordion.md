# Accordion

O componente `Accordion` é utilizado para exibir conteúdo de forma expansível e colapsável, permitindo que os usuários revejam informações de maneira organizada. Ele utiliza o componente `Disclosure` da biblioteca `@headlessui/react` para gerenciar o estado de abertura e fechamento.

## Props

### `bg` (booleano, opcional)
Define se o fundo do Accordion deve ser colorido. O valor padrão é `false`.

### `title` (string | React.ReactNode, obrigatório)
O título que será exibido no cabeçalho do Accordion. Pode ser uma string ou um elemento React.

### `children` (string | React.ReactNode, obrigatório)
O conteúdo que será exibido quando o Accordion estiver aberto. Pode ser uma string ou um elemento React.

### `fullWidth` (booleano, opcional)
Define se o Accordion deve ocupar a largura total do contêiner. O valor padrão é `undefined`.

## Exemplo de Uso

```jsx
<Accordion title="Título do Accordion" bg={true}>
  <p>Este é o conteúdo do Accordion.</p>
</Accordion>
```

## Comportamento

- O componente utiliza um botão que, ao ser clicado, alterna entre abrir e fechar o conteúdo.
- O ícone `ChevronDownIcon` muda de orientação dependendo do estado do Accordion (aberto ou fechado).
- O conteúdo é animado durante a transição de abertura e fechamento, proporcionando uma experiência de usuário suave.

## Dependências

- `@headlessui/react`: Para o gerenciamento do estado do Accordion.
- `@heroicons/react`: Para o ícone de seta que indica o estado do Accordion.
- `Container`: Componente que envolve o Accordion, permitindo controle sobre a largura.