# FaceID-TextInImage-VisionStudio-Azure-DIO

Neste LAB, o desaio foi a criação de reconhecimento facial, identificação de dados em documentos e também o reconhecimento de elementos em imagens utilizando o Vision Studio no Microsoft Azure AI + Machine Learning. Esses exercícios tem como objetivo melhorar nossas habilidades na aplicação prática de tecnologias de reconhecimento, proporcionando uma compreensão mais profunda e prática desses conceitos essenciais.


#***Detectar rostos no Vision Studio***

As soluções de visão geralmente exigem que a IA seja capaz de detectar rostos humanos. Suponha que a empresa varejista fictícia Northwind Traders queira localizar onde os clientes estão em uma loja para melhor atendê-los. Uma maneira de fazer isso é determinar se há algum rosto nas imagens e, em caso afirmativo, retornar as coordenadas da caixa delimitadora que mostram sua localização.

Para testar as capacidades de deteção facial do serviço Azure AI Face, utilizará o [Azure Vision Studi0](https://portal.vision.cognitive.azure.com/gallery/featured) . Esta é uma plataforma baseada em UI que permite explorar os recursos do Azure AI Vision sem a necessidade de escrever nenhum código.

#***Crie um recurso de serviços de IA do Azure***
Você pode usar o serviço Azure AI Face com um recurso multisserviço de serviços de IA do Azure . Se ainda não o fez, crie um recurso de serviços de IA do Azure na sua assinatura do Azure.

1. Em outra guia do navegador, abra o portal do Azure em https://portal.azure.com , entrando com a conta da Microsoft associada à sua assinatura do Azure.

2. Clique no botão **＋Criar um recurso** e pesquise os serviços de IA do Azure . Selecione **criar** um plano de serviços de IA do Azure . Você será levado a uma página para criar um recurso **de serviços de IA do Azure**. Configure-o com as seguintes configurações:

  + **Assinatura** : sua assinatura do Azure .
  + **Grupo de recursos** : Selecione ou crie um grupo de recursos com um nome exclusivo .
  + **Região** : Leste dos EUA.
  + **Nome** : Insira um nome exclusivo .
  + **Nível de preços** : Padrão S0.
  + **Ao marcar esta caixa, confirmo que li e compreendi todos os termos abaixo** : Selecionado .

3. Selecione **Revisar** **+ criar** e depois **Criar** e aguarde a conclusão da implantação.

# ***Conecte seu recurso de serviço de IA do Azure ao Vision Studio***

Em seguida, conecte o recurso de serviços de IA do Azure provisionado acima ao Vision Studio.

1. Em outra guia do navegador, navegue até **Vision Studio** em [](https://portal.vision.cognitive.azure.com).

2. Entre com sua conta e certifique-se de usar o mesmo diretório onde você criou seu recurso de serviços de IA do Azure.

3. Na página inicial do Vision Studio, selecione **Visualizar todos os recursos** no título **Introdução ao Vision** .
   
![imagem começar com o vision studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/media/analyze-images-vision/vision-resources.png)

4. Na página Selecione um recurso para trabalhar , passe o cursor do mouse sobre o recurso que você criou acima na lista e marque a caixa à esquerda do nome do recurso e selecione Selecionar como recurso padrão .

> ! **Nota** : *Se o seu recurso não estiver listado, pode ser necessário atualizar a página.*

![](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/media/analyze-images-vision/default-resource.png)

5. Feche a página de configurações selecionando o “x” no canto superior direito da tela.

#***Detecte rostos no Vision Studio***

1. Num navegador web, navegue até **Vision Studio** em https://portal.vision.cognitive.azure.com .

2. Na página **inicial Introdução ao Vision** , selecione a guia **Face** e, em seguida, selecione o bloco **Detectar rostos em uma imagem** .

3. No subtítulo **Experimente** , reconheça a política de uso de recursos lendo e marcando a caixa.

4. Selecione cada uma das imagens de amostra e observe os dados de detecção facial retornados.

5. Agora vamos tentar com algumas de nossas próprias imagens. Vá té a pasta inputs nesse repositório para baixar pegar o caminho das imagens utilizadas no exercício. 

6. Localize o arquivo chamado ....... ; que contém a seguinte imagem:

![]()

7. Faça upload de ........... e revise os detalhes de detecção de rosto retornados.

8. Localize o arquivo chamado ........... ; que contém a seguinte imagem:

![]()

9. Faça upload de .......... e revise os detalhes de detecção de rosto retornados.

10. Localize o arquivo chamado ........... ; que contém a seguinte imagem:

![]()

12. Faça upload de store-camera-3.jpg e revise os detalhes de detecção de rosto retornados. Observe como o Azure AI Face não detectou o rosto que está obscurecido.

Neste exercício você explorou como os serviços de IA do Azure podem detectar rostos em imagens. Se você tiver tempo, sinta-se à vontade para experimentar as imagens de exemplo ou algumas de suas próprias imagens.

#***Limpar***
Se não pretende fazer mais exercícios, exclua todos os recursos que não precisa mais. Isso evita acumular custos desnecessários.

Abra o **portal do Azure** em [](https://portal.azure.com) e selecione o grupo de recursos que contém o recurso que você criou.
Selecione o recurso e selecione **Excluir** e depois **Sim** para confirmar. O recurso é então excluído.

# **Saber mais**
Para saber mais sobre o que você pode fazer com este serviço, consulte a [página do serviço Azure AI Face](https://learn.microsoft.com/pt-br/azure/ai-services/computer-vision/overview-identity) .
