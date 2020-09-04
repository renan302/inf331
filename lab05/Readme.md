# Web como Plataforma e Subcomponentes
*Lab de Componentização e Reúso de Software 29/08/2020*

## Tarefa 1

  ![Tarefa1](images/image1.jpg)

## Tarefa 2

> <div id="root"></div>
> const Setvalue = () => {
>    const [name, setName] = React.useState();
>    return (<div><input type="text" placeHolder="Digite um texto" onChange={(e) => setName(e.target.value)} /> <br /><h2>{name}</h2></div>)}
>
> const elemento = <Setvalue />
>
> ReactDOM.render(elemento,
>    document.getElementById("root"));
