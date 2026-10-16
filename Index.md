# Política de Privacidade — GPS Bússola

**Última atualização:** Outubro de 2026

A sua privacidade é uma prioridade fundamental. Esta Política de Privacidade descreve de forma clara e transparente como o aplicativo **GPS Bússola** trata as informações coletadas, processadas e armazenadas durante a sua utilização, em estrita conformidade com a Lei Geral de Proteção de Dados (LGPD — Lei nº 13.709/2018), o Regulamento Geral sobre a Proteção de Dados da União Europeia (GDPR) e as diretrizes da Google Play Store.

---

### 1. Dados de Localização e GPS (Princípio de Minimização e Privacidade Offline)

O **GPS Bússola** é uma ferramenta de navegação terrestre, marítima e orientação tática. Para prestar os seus serviços essenciais, o aplicativo requer acesso aos dados de localização geográfica do seu dispositivo.

* **Localização Precisa em Primeiro Plano (Foreground):** Utilizada para determinar as coordenadas geográficas (latitude, longitude e altitude), cálculo de rumo, calibração da declinação magnética e exibição da bússola em tempo real.
* **Gravação Contínua de Trilhas (Foreground Service):** Caso você opte ativamente por iniciar a gravação de uma trilha ou trajeto, o aplicativo utilizará um Serviço em Primeiro Plano (*Foreground Service* do tipo `location`) acompanhado de uma notificação permanente visível na barra de status. Isso permite o registro contínuo da rota mesmo com a tela apagada ou com o aplicativo minimizado.
* **Sem Rastreamento Oculto em Segundo Plano:** O aplicativo **não** coleta nem monitora a sua localização em segundo plano de forma oculta ou sem o seu conhecimento deliberado.
* **Armazenamento 100% Local:** Suas coordenadas, pontos salvos (waypoints), rotas e arquivos GPX são gravados exclusivamente na base de dados interna do seu aparelho (`Room Database`). **Nenhuma coordenada pessoal ou histórico de deslocamento é enviado, comercializado ou sincronizado com servidores próprios do desenvolvedor.**

---

### 2. Rede Local e Conectividade Sem Fio (Nearby Connections e Bluetooth)

Para o funcionamento do módulo **Chat SOS / Comunicação Offline**, o aplicativo utiliza a API Google Nearby Connections via Bluetooth e Wi-Fi Direct:

* **Finalidade Exclusiva:** Permitir a troca de mensagens de texto e balizas de emergência diretamente entre dispositivos próximos em áreas sem cobertura de internet móvel ou celular (comunicação ponto a ponto / P2P).
* **Consentimento Manual e Handshake:** Nenhuma conexão é estabelecida de forma automática ou silenciosa. Cada solicitação de emparelhamento exige confirmação manual bilateral por meio de código numérico de segurança (*authentication digits*).
* **Isolamento de Uso:** As permissões de rádio (Bluetooth e Wi-Fi) são utilizadas exclusivamente para enlace de dados local, com a flag `neverForLocation` ativa, não sendo aproveitadas para inferência de localização pessoal.

---

### 3. Serviços Externos e Chamadas de Rede

Para enriquecer a experiência com dados meteorológicos, ambientais e cartográficos, o aplicativo realiza consultas a serviços terceiros especializados:

* **Esri ArcGIS Location Platform:** Utilizado para o fornecimento de camadas cartográficas (mapas topográficos e imagens de satélite). O tráfego de dados restringe-se ao carregamento dos blocos de mapa necessários para a visualização, respeitando os termos de uso da Esri.
* **Open-Meteo API & WAQI (World Air Quality Index):** Consultas anônimas baseadas na latitude e longitude arredondadas para fornecer previsões de tempo, índice de qualidade do ar (IQAr / CONAMA 491/2018) e dados do modelo Copernicus DEM para calibração de altitude. Nenhum dado pessoal identificável é anexado a essas requisições.
* **AviationWeather.gov & NOAA SWPC:** Utilizados para obtenção pública de relatórios meteorológicos de aeródromos (METAR) e índices geomagnéticos planetários (Kp / clima espacial), sem qualquer rastreamento individual.

---

### 4. Publicidade e Monetização (Google AdMob e UMP SDK)

Para viabilizar a manutenção e o desenvolvimento contínuo, o aplicativo exibe anúncios através do **Google AdMob** (Google LLC):

* **Formato e Localização:** Anúncios em formato de banner adaptativo são exibidos apenas em telas de consulta secundárias (como a lista de itens salvos). A tela principal da bússola e os visores de navegação em tempo real permanecem integralmente livres de propagandas. Anúncios intersticiais são exibidos de forma pontual e controlada, exclusivamente em transições de ação concluída (ex.: ao finalizar a gravação de um trajeto).
* **Gestão de Consentimento (Google UMP SDK):** O aplicativo integra a plataforma oficial de mensagens de consentimento do Google (*User Messaging Platform*). Em regiões cobertas pelo GDPR (União Europeia/Reino Unido) ou legislações aplicáveis como a LGPD, o usuário tem a opção de aceitar, recusar ou personalizar o compartilhamento de identificadores de publicidade para anúncios personalizados.
* **Identificadores de Anúncios:** O SDK do AdMob pode coletar identificadores de dispositivo, endereço IP aproximado e dados de interação com anúncios para fins de prevenção de fraudes, relatórios de tráfego e veiculação de publicidade em conformidade com as [Políticas de Privacidade do Google](https://policies.google.com/privacy).

---

### 5. Arquivos, Exportação e Cópia de Segurança (Backup)

* **Exportação GPX:** A geração e o compartilhamento de arquivos de trilhas no formato padrão `.gpx` são realizados de forma segura através do `Android FileProvider`, com acesso estritamente restrito à subpasta designada (`gpx_exports/`).
* **Regras de Backup:** O aplicativo adota políticas formais de exclusão de backup na nuvem para arquivos temporários e caches voláteis, protegendo a integridade dos seus dados sensíveis de navegação.

---

### 6. Direitos do Titular de Dados (LGPD e GDPR)

Em conformidade com a legislação vigente, você tem o direito de:
1. Confirmar a existência de tratamento de dados;
2. Acessar, corrigir ou solicitar a exclusão de todos os seus waypoints e trajetos diretamente na tela "Salvos" do aplicativo;
3. Revogar permissões concedidas de GPS, Câmera ou Bluetooth a qualquer momento diretamente nas configurações de aplicativos do sistema operacional Android;
4. Modificar suas preferências de consentimento de publicidade e cookies.

---

### 7. Contato e Responsável pelo Tratamento

Se você tiver dúvidas, sugestões ou solicitações relativas a esta Política de Privacidade ou ao tratamento de dados do aplicativo, entre em contato através do canal de suporte:

* **Responsável:** Desenvolvedor Jorge Henrique
* **E-mail de Suporte:** jorgehenrique2386@gmail.com
* **Localidade:** Rio de Janeiro — RJ, Brasil
