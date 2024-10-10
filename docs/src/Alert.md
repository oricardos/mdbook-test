# Alert

O componente `Alert` é utilizado para exibir mensagens de alerta ao usuário, com diferentes estilos e ícones baseados no tipo de alerta. Ele suporta quatro variantes: sucesso, aviso, perigo e informação.

## Props

O componente `Alert` aceita as seguintes propriedades:

| Nome      | Tipo                     | Descrição                                                                 |
|-----------|--------------------------|---------------------------------------------------------------------------|
| `title`   | `string`                 | O título da mensagem de alerta.                                          |
| `message` | `string | React.ReactNode` | A mensagem a ser exibida, que pode ser uma string ou um elemento React. |
| `color`   | `'success' \| 'warning' \| 'danger' \| 'info'` | Define a variante do alerta e o estilo associado.                       |
| `fullWidth` | `boolean` (opcional)   | Se verdadeiro, o alerta ocupará toda a largura disponível.              |

## Exemplo de Uso

```jsx
<Alert 
  title="Sucesso!" 
  message="Seu cadastro foi realizado com sucesso." 
  color="success" 
/>
```

## Estilos

O componente aplica diferentes classes CSS com base na propriedade `color`:

- **Ícones**:
  - `success`: CheckCircleIcon
  - `warning`: ExclamationTriangleIcon
  - `danger`: XCircleIcon
  - `info`: InformationCircleIcon

- **Classes de fundo**:
  - `success`: `bg-green-50`
  - `warning`: `bg-yellow-50`
  - `danger`: `bg-red-50`
  - `info`: `bg-blue-50`

- **Classes de título**:
  - `success`: `text-green-700`
  - `warning`: `text-yellow-700`
  - `danger`: `text-red-700`
  - `info`: `text-blue-700`

- **Classes de mensagem**:
  - `success`: `text-green-500`
  - `warning`: `text-yellow-500`
  - `danger`: `text-red-500`
  - `info`: `text-blue-500`

## Considerações

O componente `Alert` deve ser utilizado dentro de um contêiner que suporte a propriedade `fullWidth` para garantir que o alerta seja exibido corretamente em diferentes layouts.