# Especificações técnicas de backend do Módulo de Depoimentos

## Interface administrativa
Você deverá implementar uma interface administrativa na qual o administrador da loja poderá cadastrar os depoimentos, contendo nome, comentário, foto,  data do depoimento e rede social. Utilize a interface administrativa do Magento 2 para criar esta interface (veja a [documentação](https://www.mageplaza.com/magento-2-module-development/create-system-xml-configuration-magento-2.html))


A interface administrativa deve conter as funcionalidades a seguir:

### Cadastrar depoimentos
Deve ser possível cadastrar os depoimentos que foram feitos em redes sociais sobre a loja atendendo as seguintes informações:

* **Nome:** Nome do usuário que realizou o depoimento na rede ocial (obrigatório)
* **Comentário:** Depoimento escrito pelo usuário que realizou o depoimento na rede social (obrigatório)
* **Foto:** Foto do usuário que realizou o depoimento na rede social, em caso em que o usuário não tenha, aplicar a logo da loja
* **Data do depoimento:** Data em que o depoimento ocorreu (obrigatório)
* **Rede social:** A rede social em que o depoimento ocorreu (obrigatório)

### Listar depoimentos
Lista todos os depoimentos em uma grid (veja a [documentação](https://devdocs.magento.com/guides/v2.4/extension-dev-guide/admin-grid.html))

#### Filtros
* Nome (termo de pesquisa)
* Data (termo de pesquisa)
* Rede Social (termo de pesquisa)

### Editar depoimentos
Deve ser possível editar os depoimentos já cadastrados.

### Excluir depoimentos
Deve ser possível excluir os depoimentos, tanto dentro da página do depoimento quanto como uma ação em massa, ou seja realizar a exclusão de múltiplos depoimentos na grid.

### Ativar/Desativar depoimentos
Deve ser possível ativar ou desativar um depoimento, se ativado ele deve ser exibido no frontend, se desativado, não. Essa opção também deve possuir uma ação em massa na grid.
