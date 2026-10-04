# Política de Privacidade do GeoSweeper

**Data de vigência:** 26 de setembro de 2026

**Última atualização:** 4 de outubro de 2026

## A versão resumida

O GeoSweeper não coleta, transmite, vende nem compartilha nenhuma informação pessoal. Cada tabuleiro que você joga, cada configuração que você escolhe e cada país que você já limpou ficam armazenados apenas no seu dispositivo. Nada é enviado para nós, e não existe conta para criar, para começar. O único tráfego de rede que o GeoSweeper gera é a comunicação do StoreKit com a Apple quando você faz ou restaura uma compra, e páginas que você abre deliberadamente a partir de um link dentro do app (este site, ou as próprias páginas legais da Apple) — ambos são detalhados abaixo, e nenhum dos dois carrega mais nada além disso.

## Quem somos

O GeoSweeper é desenvolvido por Ivan Cayabyab. Dúvidas sobre esta política ou sobre o app podem ser enviadas para ivnsjdev@gmail.com.

## O que o app armazena, e onde

Tudo abaixo vive apenas no seu dispositivo, em um de três lugares: `UserDefaults` (pequenos valores de configuração), um arquivo JSON na pasta Application Support do próprio app, ou um banco de dados SQLite local.

| O quê | Armazenamento principal | Enviado automaticamente para nós? |
|---|---|---|
| Configurações de exibição — tema do tabuleiro, cor de neon, efeito de explosão, som de explosão, projeção do mapa (Globe ou Flat), som e resposta tátil ativados/desativados | `UserDefaults` | Não |
| Idioma escolhido dentro do app | `UserDefaults` | Não |
| Controle interno do pedido de avaliação — as datas em que o GeoSweeper pediu ao iOS para mostrar a tela nativa de avaliação, e qual marco disparou o último pedido | `UserDefaults` | Não |
| Contadores de jogos gratuitos — quantos dos seus 10 países gratuitos do mapa e dos seus 10 jogos gratuitos do **Classic** você já usou | `UserDefaults` | Não |
| Recorde por país — vitórias, derrotas, melhor tempo e quando você o desbloqueou, para cada país que você já jogou | Um arquivo JSON (`progress.json`) na pasta Application Support do app | Não |
| Histórico do modo **Classic** — o tamanho do tabuleiro, a dificuldade, a quantidade de minas, o tempo e a vitória ou derrota de cada jogo do Classic concluído | Um arquivo JSON (`Classic/history.json`) na pasta Application Support do app | Não |
| Progresso da Infinite Tower — a fileira que você alcançou, sua posição de visualização salva e quais fileiras você já limpou | Um banco de dados SQLite local | Não |

Nada disso é transmitido, vendido ou compartilhado com ninguém, inclusive nós. O tráfego próprio do StoreKit (abaixo) e os links externos que você toca (também abaixo) não carregam nada disso. Um backup do dispositivo iOS pode incluir esses arquivos como parte do backup do app como um todo — esse backup é iniciado por você ou pelo iOS, nunca pelo GeoSweeper, e permanece onde você o enviar (iCloud ou seu computador), não conosco.

## Sem conta, sem login, sem nuvem

O GeoSweeper nunca pede nome, endereço de e-mail, número de telefone, data de nascimento ou qualquer outra informação de identificação — não há nada para fazer login, porque não existe conta. Seu progresso não sincroniza via iCloud, CloudKit ou qualquer outro serviço: ele vive apenas no dispositivo em que você está jogando. Jogue o mesmo país em um segundo dispositivo e ele começará do zero ali, porque não existe nenhuma cópia em servidor de onde sincronizar.

## O que deliberadamente não é salvo

O tabuleiro em que você está no meio do jogo — cada casa aberta, cada bandeira colocada — fica apenas na memória enquanto você joga. Isso vale para os três mundos: o mapa, o modo **Classic** e a **Infinite Tower**. Feche o app no meio de uma partida e esse tabuleiro desaparece; ele nunca é gravado em disco, e não existe salvamento automático para retomar um tabuleiro inacabado. Só um jogo *terminado* (uma vitória ou uma derrota) atualiza o recorde por país ou o histórico do Classic descritos acima.

## A única coisa que parece não ser local

O mapa abre no seu próprio país na primeira vez que você inicia o app. Isso vem da **configuração de região** do seu dispositivo (o país vinculado ao seu idioma e localidade, o mesmo que o iOS usa para escolher um teclado e um calendário) — não de GPS, Wi-Fi ou qualquer outra forma de rastreamento de localização. O GeoSweeper não solicita acesso à localização e não conseguiria ler suas coordenadas mesmo que quisesse.

## Permissões

O GeoSweeper não solicita nenhuma permissão do sistema. Ele nunca pede acesso à câmera, à biblioteca de fotos, ao microfone, à localização, aos contatos, ao calendário, a dados de saúde, a dados de movimento ou a notificações push, e nenhum tipo de solicitação de permissão jamais aparecerá. Isso corresponde exatamente ao `Info.plist` do app: não há uma única entrada de descrição de uso nele.

## Compras

O GeoSweeper é gratuito para baixar, e cada um dos seus três mundos tem seu próprio período de teste gratuito. Seus primeiros 10 países no mapa — de qualquer nível, incluindo Beginner — são gratuitos para jogar, e depois que você joga um país, ele permanece jogável para sempre, mesmo depois que esse teste acabar. O modo **Classic** dá a você 10 jogos gratuitos da mesma forma. A Infinite Tower é gratuita até a fileira 10. Além desses pontos, existem três compras independentes, todas únicas, não consumíveis, oferecidas através do StoreKit da Apple e processadas inteiramente pela Apple:

- **All Countries** — uma compra única, não consumível, que desbloqueia permanentemente os níveis Intermediate, Expert e Mega em todos os 204 países. Nada nisso é renovado.
- **Classic Lifetime** — uma compra única, não consumível, que desbloqueia permanentemente jogos ilimitados do Classic depois que seus 10 gratuitos acabarem. Nada nisso é renovado.
- **Infinite Tower Lifetime** — uma compra única, não consumível, que desbloqueia permanentemente subir além da fileira 10. Isso também nunca é renovado, e o GeoSweeper não oferece nenhum tipo de assinatura.

A Apple, não o GeoSweeper, processa todo pagamento. Nenhum número de cartão, endereço de cobrança ou credencial da Apple Account é visível para nós em nenhum momento — o StoreKit só informa ao app o que ele precisa para mostrar uma tela de compra e conceder acesso: o preço a exibir, e se você já possui cada item. Essas respostas ficam no seu dispositivo; o GeoSweeper não opera um servidor de compras próprio e não tem para onde enviá-las. Restaurar compras pede à Apple para reconfirmar o que sua Apple Account possui e aplica a resposta localmente — isso não cria nem transmite nenhum registro novo.

Veja também o [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/) da Apple, os [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) e o [Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), que regem a compra em si.

## Comunicações de suporte

Se você enviar um e-mail para ivnsjdev@gmail.com, recebemos seu endereço de e-mail, o que você escrever e qualquer anexo que você decidir incluir. Usamos isso apenas para responder você e resolver o problema sobre o qual você escreveu — nossa base legal é nosso interesse legítimo em responder às pessoas que entram em contato conosco. Essa caixa de entrada é uma conta padrão do Gmail, processada pela Google LLC conforme a [Google's Privacy Policy](https://policies.google.com/privacy), e hospedada em infraestrutura que pode estar localizada fora do seu país, por isso essa transferência é divulgada aqui. Mantemos e-mails de suporte por até 24 meses e depois os excluímos; você pode nos pedir para excluir um e-mail específico antes disso a qualquer momento, escrevendo para o mesmo endereço.

## Links externos

As telas de compra do GeoSweeper linkam para a política de privacidade deste site e para o Standard EULA da Apple; a tela Settings pode linkar para a página de avaliação da App Store. Nenhum dado do usuário ou identificador específico do app é adicionado a nenhum desses links — são URLs simples, iguais para todo mundo.

## Nada para apostar

O GeoSweeper não tem moeda interna, itens sorteados, sorteios de prêmios nem qualquer recurso em que um resultado seja apostado. Toda compra é um preço fixo e divulgado por acesso permanente ou por tempo limitado a conteúdo; nada pode ser ganho, perdido ou apostado.

## O que NÃO fazemos

- Nenhuma análise (analytics), relatório de falhas ou telemetria de qualquer tipo
- Nenhuma publicidade, nenhuma rede de anúncios e nenhum identificador de publicidade
- Nenhum rastreamento entre apps ou entre sites, e nenhum corretor de dados
- Nenhuma conta, nenhum login, nenhuma senha
- Nenhum acesso a câmera, biblioteca de fotos, microfone, contatos, localização precisa ou aproximada, ou dados de saúde
- Nenhum treinamento de modelos de aprendizado de máquina com seus dados
- Nenhum SDK de terceiros de qualquer tipo — o único código neste app é nosso

Isso corresponde ao selo "Data Not Collected" (dados não coletados) que o GeoSweeper carrega na App Store.

## Retenção e exclusão

Excluir o app apaga todos os arquivos que ele armazenou no seu dispositivo — configurações, seu recorde por país, seu histórico do modo Classic e seu progresso na Infinite Tower — imediata e completamente, porque nunca existiu uma cópia em servidor para mantermos ou excluirmos do nosso lado. Um backup do iCloud feito antes da exclusão ainda pode conter uma cópia; esse backup está totalmente sob seu controle em **Ajustes → seu nome → iCloud → Gerenciar Armazenamento da Conta** no seu dispositivo. E-mails de suporte são retidos e excluídos separadamente, conforme descrito acima.

## Seus direitos

Como o GeoSweeper não mantém nenhuma cópia dos seus dados dentro do app, os direitos de acesso, correção, exportação e exclusão descritos pelo GDPR, pelo UK GDPR e pela CCPA/CPRA são direitos que você já exerce diretamente, no seu próprio dispositivo — não há nenhum registro aqui para produzirmos ou apagarmos em seu nome. O único lugar em que guardamos algo é um e-mail de suporte que você nos enviou, e você pode pedir para ver, corrigir ou excluir isso a qualquer momento, escrevendo para ivnsjdev@gmail.com. Não vendemos nem compartilhamos informações pessoais para publicidade comportamental entre contextos, e nunca vendemos. Se você acredita que tratamos seus dados de forma inadequada, você tem o direito de registrar uma reclamação junto à sua autoridade local de proteção de dados.

## Crianças

O GeoSweeper tem uma classificação etária adequada para o público em geral e não é direcionado especificamente a crianças. Não coletamos intencionalmente informações pessoais de ninguém, incluindo crianças menores de 13 anos, e não há nada no app que pudesse fazer isso — nenhum chat, nenhum compartilhamento, nenhum recurso social, nenhuma publicidade e nenhuma conta pela qual terceiros pudessem alcançar uma criança.

## Alterações nesta política

Se esta política mudar, a data no topo mudará junto com ela, e uma alteração material no que o GeoSweeper faz com dados também será mencionada nas notas de versão dessa atualização.

## Contato

ivnsjdev@gmail.com
