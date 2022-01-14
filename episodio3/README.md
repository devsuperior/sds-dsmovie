# ![DevSuperior logo](https://raw.githubusercontent.com/devsuperior/bds-assets/main/ds/devsuperior-logo-small.png) Semana Spring React - Episódio 3
>  *Crie um app inédito para seu portfólio com as tecnologias mais demandadas do mercado*

## Realização
[DevSuperior - Escola de programação](https://devsuperior.com.br)

[![DevSuperior no Instagram](https://raw.githubusercontent.com/devsuperior/bds-assets/main/ds/ig-icon.png)](https://instagram.com/devsuperior.ig)
[![DevSuperior no Youtube](https://raw.githubusercontent.com/devsuperior/bds-assets/main/ds/yt-icon.png)](https://youtube.com/devsuperior)

## Objetivos do projeto para esta aula
- Integrar back end e front end
- Três pilares do React
  - Componentes
  - Props
  - Estado
- React Hooks
  - useState
  - useEffect
  - useParams
  - useNavigate

## AVISO: as aulas ficarão disponíveis somente até domingo às 23h59

## AVISO: Instruções sobre certificado no Github do [aqui](https://github.com/devsuperior/sds-dsmovie/tree/main/_certificado)

### Passo: Primeira requisição

- Instalar Axios
```bash
yarn add axios@0.24.0
```
- Definir BASE_URL
- Definir os tipos Movie e MoviePage
- Fazer a requisição

```typescript
export type Movie = {
    id: number;
    title: string;
    score: number;
    count: number;
    image: string;
}

export type MoviePage = {
    content: Movie[];
    last: boolean;
    totalPages: number;
    totalElements: number;
    size: number;
    number: number;
    first: boolean;
    numberOfElements: number;
    empty: boolean;
}
```

- **COMMIT: First request**

### Passo: React hooks: useState e useEffect

Hooks são funções cujo comportamento está vinculado ao estado e ao ciclo de vida do React a partir de componentes funcionais.

https://pt-br.reactjs.org/docs/hooks-overview.html

```
Hook: useState
Manter estado no componente
```
```
Hook: useEffect
Executar algo na instanciação ou destruição do componente, observar estado
```

- **COMMIT: useState, useEffect**

### Passo: Props

Props podem ser entendidas como argumentos do componente React.

https://pt-br.reactjs.org/docs/components-and-props.html

NOTA: em uma renderização dinâmica de coleção, cada elemento renderizado DEVE possuir um atributo `key`.

- **COMMIT: Props**

### Passo: useParams

- **COMMIT: useParams**


### Passo: Mostrar estrelinhas
```js
// EX:
// getFills(3.5) => [1, 1, 1, 0.5, 0]
// getFills(4.1) => [1, 1, 1, 1, 0.5]
function getFills(score: number) {

  const fills = [0, 0, 0, 0, 0];

  const integerPart = Math.floor(score);

  for (let i = 0; i < integerPart; i++) {
    fills[i] = 1;
  }

  const diff = score - integerPart;
  if (diff > 0) {
    fills[integerPart] = 0.5;
  }

  return fills;
}
```


- **COMMIT: Show score**


### Passo: Pagination

- Controlar botão habilitado/desabilitado
- Trocar página ao clique do botão

```js
const handlePageChange = (newNumber: number) => {
    setPageNumber(newNumber);
}
```

- **COMMIT: Pagination**


### Passo: Salvando score, useNavigate

# ATENÇÃO: Coloque o [movieId] nas dependências o useEffect do FormCard:
```js
useEffect(() => {
    axios.get(`${BASE_URL}/movies/${movieId}`)
        .then(response => {
            setMovie(response.data);
        });
}, [movieId]);
```

Função para validar email

```javascript
// https://stackoverflow.com/questions/46155/whats-the-best-way-to-validate-an-email-address-in-javascript
export function validateEmail(email: any) {
  return String(email)
    .toLowerCase()
    .match(
      /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/
    );
}
```

Objeto de configuração da requisição Axios

```
const config: AxiosRequestConfig = {
	baseURL: BASE_URL,
	method: 'PUT',
	url: '/scores',
	data: {
		email: email,
		movieId: movieId,
		score: score
	}
}
```

- **COMMIT: Save, useNavigate**



## PARABÉNS!

![Parabéns!](https://raw.githubusercontent.com/devsuperior/bds-assets/main/img/trophy.png)

- Quero muito saber seu feedback
  - O que você está achando da nossa abordagem?
  - Você está conseguindo acompanhar?
  - O que você está achando do evento?
- Participe
  - Comente na página da Semana Spring React
  - Divulgue seu projeto no Linkedin e marque a DevSuperior

