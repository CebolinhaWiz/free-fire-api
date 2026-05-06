# 📝 Documentação da API

## API de Informações do Jogador
Rota da API = https://free-fire-data.vercel.app/api/data?region={region}&uid={uid}&key={key}

**Endpoint:** `api/data`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint recupera informações do jogador com base na região e ID de usuário especificados.

### 📨 Exemplo de Requisição
```http
GET https://free-fire-data.vercel.app/api/data?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parâmetros de Consulta

| Parâmetro | Tipo   | Obrigatório | Descrição                          |
|-----------|--------|-------------|------------------------------------|
| `region`  | string | Sim         | O código da região (`sg`, `ind`, `br`) |
| `uid`     | int    | Sim         | O ID do usuário                   |
| `key`     | string | Sim         | Compre a chave em https://t.me/B10_NET |

### ℹ️ Nota Importante

Parâmetro de consulta `SG` é para todas as regiões que estão sob `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parâmetro de consulta `IND` é apenas para a Índia e está sob `client.ind.freefiremobile.com`  
[`IND`]

Parâmetro de consulta `BR` é para todas as regiões que estão sob `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Exemplo de uma Resposta Bem-Sucedida Pode Ser Assim,
```json
{
  "basicInfo": {
    "accountId": 2129250963,
    "accountType": 1,
    "bannerId": 901026021,
    "bpStatus": null,
    "brMaxRank": 316,
    "brRank": 2768,
    "createAt": 1747304828,
    "csMaxRank": 316,
    "csRank": 45,
    "exp": 133627,
    "headPic": 902000057,
    "lastLoginAt": 1593158767,
    "level": 42,
    "liked": 4957,
    "nickname": "JOAOKL 500K",
    "region": "IND",
    "releaseVersion": "OB48",
    "showBrRank": true,
    "showCsRank": true,
    "title": 904090024
  },
  "captainBasicInfo": {
    "accountId": 2129250963,
    "accountType": 1,
    "badgeCnt": 42,
    "bannerId": 901026021,
    "brMaxRank": 316,
    "brRank": 316,
    "brRankingPoints": 2768,
    "createAt": 1593158767,
    "csMaxRank": 305,
    "csRank": 305,
    "csRankingPoints": 17,
    "exp": 133627,
    "headPic": 902000057,
    "lastLoginAt": 1747304828,
    "level": 42,
    "liked": 4957,
    "nickname": "JOAOKL 500K",
    "region": "IND",
    "releaseVersion": "OB48",
    "seasonId": 45
  },
  "clanBasicInfo": [
    {
      "capacity": 25,
      "captainId": 2129250963,
      "clanId": 3000167557,
      "clanLevel": 1,
      "clanName": "〆ᗷᖇᝪᎢᕼᗴᖇ",
      "memberNum": 5
    }
  ],
  "creditScoreInfo": {
    "creditScore": 100,
    "periodicSummaryEndTime": 1747564036,
    "periodicSummaryStartTime": 1747304836,
    "rewardState": 2
  },
  "petInfo": {
    "exp": 548,
    "id": 1300000120,
    "level": 4,
    "nickname": null,
    "selectedSkillId": 1310000201,
    "skinId": 1315000010
  },
  "socialInfo": {
    "accountId": 2129250963,
    "brRankShow": 1,
    "csRankShow": null,
    "signature": "JoaoKL Never Dies."
  }
}
```

## API de Estatísticas do Jogador
Rota da API = https://free-fire-data.vercel.app/api/stats?region={region}&uid={uid}&key={key}

**Endpoint:** `api/stats`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint recupera informações de estatísticas do jogador com base na região e ID de usuário especificados.

### 📨 Exemplo de Requisição
```http
GET https://free-fire-data.vercel.app/api/stats?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parâmetros de Consulta

| Parâmetro | Tipo   | Obrigatório | Descrição                          |
|-----------|--------|-------------|------------------------------------|
| `region`  | string | Sim         | O código da região (`sg`, `ind`, `br`) |
| `uid`     | int    | Sim         | O ID do usuário                   |
| `key`     | string | Sim         | Compre a chave em https://t.me/B10_NET |

### ℹ️ Nota Importante

Parâmetro de consulta `SG` é para todas as regiões que estão sob `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parâmetro de consulta `IND` é apenas para a Índia e está sob `client.ind.freefiremobile.com`  
[`IND`]

Parâmetro de consulta `BR` é para todas as regiões que estão sob `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Exemplo de uma Resposta Bem-Sucedida Pode Ser Assim,
```json
{
  "success": true,
  "soloStats": {
    "accountId": "10000001",
    "gamesPlayed": 2,
    "kills": 7,
    "detailedStats": {
      "deaths": 2,
      "distanceTravelled": 5309,
      "survivalTime": 587,
      "highestKills": 4,
      "damage": 1764,
      "headshots": 1,
      "headshotKills": 1,
      "pickUps": 146
    }
  },
  "duoStats": {
    "accountId": "10000001",
    "detailedStats": {

    }
  },
  "quadStats": {
    "accountId": "10000001",
    "gamesPlayed": 13,
    "wins": 3,
    "kills": 36,
    "detailedStats": {
      "deaths": 10,
      "topNTimes": 6,
      "distanceTravelled": 60689,
      "survivalTime": 9210,
      "revives": 4,
      "highestKills": 6,
      "damage": 17872,
      "headshots": 16,
      "headshotKills": 5,
      "knockDown": 42,
      "pickUps": 1536
    }
  }
}
```

## API de Curtidas
Rota da API = https://free-fire-data.vercel.app/api/like?region={region}&uid={uid}&key={key}

**Endpoint:** `api/like`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint envia 100 curtidas para a conta do jogador com base na região e ID de usuário especificados.

### 📨 Exemplo de Requisição
```http
GET https://free-fire-data.vercel.app/api/like?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parâmetros de Consulta

| Parâmetro | Tipo   | Obrigatório | Descrição                          |
|-----------|--------|-------------|------------------------------------|
| `region`  | string | Sim         | O código da região (`sg`, `ind`, `br`) |
| `uid`     | int    | Sim         | O ID do usuário                   |
| `key`     | string | Sim         | Compre a chave em https://t.me/B10_NET |

### ℹ️ Nota Importante

Parâmetro de consulta `SG` é para todas as regiões que estão sob `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parâmetro de consulta `IND` é apenas para a Índia e está sob `client.ind.freefiremobile.com`  
[`IND`]

Parâmetro de consulta `BR` é para todas as regiões que estão sob `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Exemplo de uma Resposta Bem-Sucedida Pode Ser Assim,
```json
{
  "response": {
    "KeyExpiresAt": "2025-03-20T90:30:00.696969",
    "KeyRemainingRequests": "69/100",
    "LikesGivenByAPI": 100,
    "LikesafterCommand": 6969,
    "LikesbeforeCommand": 6869,
    "PlayerLevel": 69,
    "PlayerNickname": "JOAOKL 500K",
    "UID": "2129250963"
  },
  "status": 1
}
```

## API de Visitas
Rota da API = https://free-fire-data.vercel.app/api/visit?region={region}&uid={uid}&key={key}

**Endpoint:** `api/visit`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint envia 100 visitas para a conta do jogador com base na região e ID de usuário especificados.

### 📨 Exemplo de Requisição
```http
GET https://free-fire-data.vercel.app/api/visit?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parâmetros de Consulta

| Parâmetro | Tipo   | Obrigatório | Descrição                          |
|-----------|--------|-------------|------------------------------------|
| `region`  | string | Sim         | O código da região (`sg`, `ind`, `br`) |
| `uid`     | int    | Sim         | O ID do usuário                   |
| `key`     | string | Sim         | Compre a chave em https://t.me/B10_NET |

### ℹ️ Nota Importante

Parâmetro de consulta `SG` é para todas as regiões que estão sob `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parâmetro de consulta `IND` é apenas para a Índia e está sob `client.ind.freefiremobile.com`  
[`IND`]

Parâmetro de consulta `BR` é para todas as regiões que estão sob `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Exemplo de uma Resposta Bem-Sucedida Pode Ser Assim,
```json
{
  "response": {
    "KeyExpiresAt": "2025-03-20T90:30:00.696969",
    "KeyRemainingRequests": "69/100",
    "VisitsSentByAPI": 100,
    "PlayerLevel": 69,
    "PlayerNickname": "JOAOKL 500K",
    "UID": "2129250963"
  },
  "status": 1
}
```

## API de Spam
Rota da API = https://free-fire-data.vercel.app/api/spam?region={region}&uid={uid}&key={key}

**Endpoint:** `api/spam`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint envia 100 solicitações de amizade para a conta do jogador com base na região e ID de usuário especificados.

### 📨 Exemplo de Requisição
```http
GET https://free-fire-data.vercel.app/api/spam?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parâmetros de Consulta

| Parâmetro | Tipo   | Obrigatório | Descrição                          |
|-----------|--------|-------------|------------------------------------|
| `region`  | string | Sim         | O código da região (`sg`, `ind`, `br`) |
| `uid`     | int    | Sim         | O ID do usuário                   |
| `key`     | string | Sim         | Compre a chave em https://t.me/B10_NET |

### ℹ️ Nota Importante

Parâmetro de consulta `SG` é para todas as regiões que estão sob `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parâmetro de consulta `IND` é apenas para a Índia e está sob `client.ind.freefiremobile.com`  
[`IND`]

Parâmetro de consulta `BR` é para todas as regiões que estão sob `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Exemplo de uma Resposta Bem-Sucedida Pode Ser Assim,
```json
{
  "response": {
    "KeyExpiresAt": "2025-03-20T90:30:00.696969",
    "KeyRemainingRequests": "69/100",
    "FriendRequestsSentByAPI": 100,
    "isPlayerOnline": true,
    "PlayerLevel": 69,
    "PlayerNickname": "JOAOKL 500K",
    "UID": "2129250963"
  },
  "status": 1
}
```

## API de Imagens
Rota da API = https://free-fire-data.vercel.app/api/images?iconName={iconName}&key={key}

**Endpoint:** `api/images`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint recupera informações do jogador com base na região e ID de usuário especificados.

### 📨 Exemplo de Requisição
```http
GET https://free-fire-data.vercel.app/api/images?iconName=Icon_avatar_hair_cos_eggday2021_headwear_blue&key=KEY123
```

### ☑️ Parâmetros de Consulta

| Parâmetro   | Tipo   | Obrigatório | Descrição                          |
|-------------|--------|-------------|------------------------------------|
| `iconName`  | string | Sim         | O nome do ícone.                   |
| `key`       | string | Sim         | Compre a chave em https://t.me/B10_NET |

### 💬 Exemplo de uma Resposta Bem-Sucedida Pode Ser Assim,

![Icon_avatar_hair_cos_eggday2021_headwear_blue](https://github.com/joaokl/free-fire-api/blob/main/images.png)

## API de Informações de Mapas Craftland
Rota da API = https://free-fire-data.vercel.app/api/maps?region={region}&code=%23{CODE}&key={key}

**Endpoint:** `api/maps`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint recupera informações do jogador com base na região e ID de usuário especificados.

### 📨 Exemplo de Requisição
```http
GET https://free-fire-data.vercel.app/api/maps?region=sg&code=%23FREEFIREMAPCODE6969&key=KEY123
```

### ☑️ Parâmetros de Consulta

| Parâmetro | Tipo   | Obrigatório | Descrição                          |
|-----------|--------|-------------|------------------------------------|
| `region`  | string | Sim         | O código da região (`sg`, `ind`, `br`) |
| `uid`     | int    | Sim         | O ID do usuário                   |
| `key`     | string | Sim         | Compre a chave em https://t.me/B10_NET |

### ℹ️ Nota Importante

Parâmetro de consulta `SG` é para todas as regiões que estão sob `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parâmetro de consulta `IND` é apenas para a Índia e está sob `client.ind.freefiremobile.com`  
[`IND`]

Parâmetro de consulta `BR` é para todas as regiões que estão sob `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Exemplo de uma Resposta Bem-Sucedida Pode Ser Assim,
```json
{
  "code": 0,
  "status": "success",
  "msg": "",
  "data": {
    "region_lang": "SG_en",
    "start_time": 1,
    "end_time": 1890713325,
    "rule": "Garena Free Fire",
    "region": "SG",
    "lang": "en",
    "title": "Garena Free Fire",
    "android_download_url": "https://play.google.com/store/apps/details?id=com.dts.freefireth&referrer=af_tranid%3DgTVeQgRDoYWAmOvmEZz6Xw%26pid%3DOrganicA%26c%3Dmainpage_AND%26af_web_id%3Da209618f-0ae1-4239-bed0-46bcfb0c9656-c",
    "ios_download_url": "https://apps.apple.com/US/app/id1300146617?mt=8",
    "ugc_url": "https://createofficial.garena.com/",
    "imgs": [
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND01.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND02.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND03.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND04.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND05.png"
    ],
    "game_icon": "https://dl.dir.freefiremobile.com/common/OB45/CSH/abcdfallstorebanners/appicon/FF_AndroidIcon_512.png",
    "game_name": "Free Fire: 7th Anniversary!",
    "transify": {
      "COMMON_ACCEPT": "ACEITAR",
      "COMMON_BACK": "Voltar",
      "COMMON_CANCEL": "Cancelar",
      "COMMON_CONFIRM": "Confirmar",
      "COMMON_CONTINUE_PURCHASE": "Continuar para comprar",
      "COMMON_COPY": "Copiar",
      "COMMON_COPY_FAILED": "Falha ao copiar",
      "COMMON_COPY_SUCCESS": "Cópia bem-sucedida",
      "COMMON_EXCHANGE": "Resgatar",
      "COMMON_EXCHANGED": "Resgatado",
      "COMMON_FFTOKEN_HINT": "Convertido para {num}{ícone de token ff}",
      "COMMON_FREE": "Grátis",
      "COMMON_GEM_CONFIRM": "Gastar {cost} gema(s) para comprar {NAME}?",
      "COMMON_GEM_CONFIRM2": "Gastar {cost} gemas para {num} giro(s)?",
      "COMMON_HISTORY_DRAW": "Histórico",
      "COMMON_HISTORY_NORECORDS": "Sem registros",
      "COMMON_HISTORY_PURCHASE": "Histórico de compras",
      "COMMON_HISTORY_REDEEM": "Histórico de resgates",
      "COMMON_NO": "Não",
      "COMMON_OWNED": "POSSUÍDO",
      "COMMON_PRIZEPOOL": "Piscina de recompensas",
      "COMMON_PURCHASE": "Comprar",
      "COMMON_PURCHASED": "Comprado",
      "COMMON_QUANTITY_MAX": "Máximo",
      "COMMON_REDEEM_CONFIRM": "Tem certeza de que deseja resgatar este item?",
      "COMMON_REJECT": "Recusar",
      "COMMON_RULE": "Regras",
      "COMMON_SKIP": "Pular animação",
      "COMMON_SKIPANIMATION_TIP": "Toque em qualquer lugar para pular a animação",
      "COMMON_SPIN_AGAIN": "Girar novamente",
      "COMMON_TIPS_ITEM": "As recompensas serão enviadas diretamente para o seu cofre",
      "COMMON_TIPS_TOKEN": "Tokens foram acumulados automaticamente",
      "COMMON_VISIT_GIFT": "Presente de boas-vindas",
      "COMMON_YES": "Sim",
      "POPUP_NO_REMIND": "Não me lembre novamente",
      "POPUP_TITLE_CONGRATULATIONS": "Parabéns!",
      "POPUP_TITLE_REDEEM": "Parabéns! Você conseguiu",
      "POPUP_TITLE_UNIQUE": "Os itens únicos que você possui",
      "UNIQUE_BUY_ALREADY_HAVE": "Você já possui este item, se comprá-lo novamente, ele será convertido em tokens FF",
      "UNIQUE_BUY_ALREADY_HAVE_PART": "Você já possui alguns dos itens selecionados. Se receber novamente, será convertido em tokens FF.",
      "UNIQUE_REDEEM_ALREADY_HAVE": "Você já possui este item, se recebê-lo novamente, ele será convertido em tokens FF.",
      "TOAST_ERROR_CODE": "Erro desconhecido, código de erro {code}",
      "TOAST_EVENTOVER": "Evento encerrado",
      "TOAST_EVENT_CLOSED_AWHILE": "O evento está temporariamente fechado. Por favor, verifique novamente mais tarde.",
      "TOAST_EVENT_END": "Evento encerrado",
      "TOAST_EVENT_NOTOPEN": "O evento ainda não começou",
      "TOAST_EXCHANGE_SUCCESS": "Resgatado com sucesso",
      "TOAST_GEM_NOT_ENOUGH": "Diamantes insuficientes, por favor, recarregue e volte novamente",
      "TOAST_LOGIN_FAILED": "Falha no login",
      "TOAST_NETWORK_BUSY": "Servidor ocupado, por favor, tente novamente mais tarde",
      "TOAST_NETWORK_ERROR": "Erro de conexão de rede, por favor, tente novamente mais tarde",
      "TOAST_OPERATE_BUSY": "Muitas solicitações, por favor, tente novamente mais tarde",
      "TOAST_PAY_FAILED": "Falha na compra",
      "TOAST_PURCHASE_SUCCESS": "Compra bem-sucedida",
      "TOAST_SERVER_BUSY": "Servidor ocupado, por favor, tente novamente mais tarde",
      "TOAST_SERVER_NOTWORK": "Serviço indisponível",
      "TOAST_SERVER_TIMEOUT": "Tempo limite do serviço",
      "TOAST_WRONG_REGION": "Este evento não está disponível para sua região",
      "COMMON_CALLBACK": "Junte-se à luta!",
      "COMMON_JOIN": "Entrar",
      "COMMON_SHOOT": "Toque nos alvos",
      "COMMON_SHOOT_2": "Bom trabalho! Para continuar, por favor, vá para o Free Fire!",
      "UGC_46_MAPSHARE_GOBUTTON": "EXPLORAR MAIS",
      "UGC_46_MAPSHARE_PLAYBUTTON": "JOGAR AGORA",
      "UGC_46_MAPSHARE_WRONGMESSAGE": "DESCULPE-NOS, ESTE MAPA NÃO ESTÁ DISPONÍVEL NO MOMENTO.",
      "UGC_47_MAPSHARE_MAPCODE": "Código do Mapa",
      "UGC_47_MAPSHARE_NAME": "Nome do Criador",
      "UGC_47_MAPSHARE_TOAST1": "Copiado com sucesso",
      "UGC_47_MAPSHARE_TOAST2": "Falha ao copiar"
    },
    "share_img": "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/SOFTFF.jpg",
    "desc_prefix": "[Free Fire]{desc}",
    "source_params": {
      "region": "",
      "lang": "en",
      "version": "",
      "action": "",
      "map_code": ""
    }
  }
}
```

## API de Lista de Desejos do Jogador
Rota da API = https://free-fire-data.vercel.app/api/wishlist?region={region}&uid={uid}&key={key}

**Endpoint:** `api/wishlist`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint recupera informações do jogador com base na região e ID de usuário especificados.

### 📨 Exemplo de Requisição
```http
GET https://free-fire-data.vercel.app/api/wishlist?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parâmetros de Consulta

| Parâmetro | Tipo   | Obrigatório | Descrição                          |
|-----------|--------|-------------|------------------------------------|
| `region`  | string | Sim         | O código da região (`sg`, `ind`, `br`) |
| `uid`     | int    | Sim         | O ID do usuário                   |
| `key`     | string | Sim         | Compre a chave em https://t.me/B10_NET |

### ℹ️ Nota Importante

Parâmetro de consulta `SG` é para todas as regiões que estão sob `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parâmetro de consulta `IND` é apenas para a Índia e está sob `client.ind.freefiremobile.com`  
[`IND`]

Parâmetro de consulta `BR` é para todas as regiões que estão sob `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Exemplo de uma Resposta Bem-Sucedida Pode Ser Assim,
```json
{
  "items": [
    {
      "itemId": 102000035,
      "releaseTime": 1709233149
    },
    {
      "itemId": 203000036,
      "releaseTime": 1710238335
    },
    {
      "itemId": 203000981,
      "releaseTime": 1706079412
    },
    {
      "itemId": 204033044,
      "releaseTime": 1706079412
    },
    {
      "itemId": 205033048,
      "releaseTime": 1706079412
    },
    {
      "itemId": 211000411,
      "releaseTime": 1706079412
    },
    {
      "itemId": 211000894,
      "releaseTime": 1706079412
    },
    {
      "itemId": 214000023,
      "releaseTime": 1706079412
    },
    {
      "itemId": 901040034,
      "releaseTime": 1727692721
    },
    {
      "itemId": 902000003,
      "releaseTime": 1710238335
    },
    {
      "itemId": 902040026,
      "releaseTime": 1710238335
    },
    {
      "itemId": 902040029,
      "releaseTime": 1710238335
    },
    {
      "itemId": 902040030,
      "releaseTime": 1710238335
    },
    {
      "itemId": 903040007,
      "releaseTime": 1727692721
    },
    {
      "itemId": 903043010,
      "releaseTime": 1710238335
    },
    {
      "itemId": 904040010,
      "releaseTime": 1727692721
    },
    {
      "itemId": 904090027,
      "releaseTime": 1707398570
    },
    {
      "itemId": 905039004,
      "releaseTime": 1710238335
    },
    {
      "itemId": 906036010,
      "releaseTime": 1706524016
    },
    {
      "itemId": 907102508,
      "releaseTime": 1706079412
    },
    {
      "itemId": 907104073,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104074,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104075,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104076,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104077,
      "releaseTime": 1727692721
    },
    {
      "itemId": 909040014,
      "releaseTime": 1727692721
    },
    {
      "itemId": 909043013,
      "releaseTime": 1707543814
    },
    {
      "itemId": 911004301,
      "releaseTime": 1710238335
    },
    {
      "itemId": 912037001,
      "releaseTime": 1706079412
    },
    {
      "itemId": 921047018,
      "releaseTime": 1735657844
    }
  ]
}
```


## 🏰 APIs de Guilda

## API de Informações da Guilda
Rota da API = https://free-fire-data.vercel.app/api/guildinfo?region={region}&guild_id={guild_id}&key={key}

**Endpoint:** `api/guildinfo`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint recupera informações completas de uma guilda, incluindo dados gerais e lista de jogadores.

### 📨 Exemplo de Requisição
GET https://free-fire-data.vercel.app/api/guildinfo?region=br&guild_id=61207059&key=KEY123

### 💬 Exemplo de Resposta
{
  "guilda": {
    "id": 12345678,
    "nome": "TropaEliteBR",
    "criadoEm": 1620000000,
    "donoId": 987654321,
    "nivel": 5,
    "limiteMembros": 50,
    "membrosAtuais": 47,
    "descricao": "Guilda competitiva BR",
    "regiao": "BR",
    "energiaGuilda": 18500,
    "atualizadoEm": 1778000000,
    "rankingPosicao": 120,
    "totalHonra": 3456789,
    "honraSemanal": 84500,
    "rankingGlobalPosicao": 450,
    "tipoRelacionamento": 1778482800
  },
  "jogadores": [
    {
      "player_id": 10000001,
      "nickname": "EliteX7",
      "pais": "BR",
      "level": 75,
      "experiencia": 5000000,
      "honra": 120000,
      "honraSemanal": 2500,
      "entradaNaGuilda": 1777000000,
      "gvgTotal": 300,
      "lastLoginAt": 1778050000
    }
  ]
}

---

## API de Pontuação Guerra de Guildas (GVG)
Rota da API = https://free-fire-data.vercel.app/api/gvg?region={region}&guild_id={guild_id}&key={key}

**Endpoint:** `api/gvg`  
**Método:** `GET`  

Este endpoint recupera a pontuação dos membros da guilda que participaram do evento Guerra de Guildas.

### 📨 Exemplo de Requisição
GET https://free-fire-data.vercel.app/api/gvg?region=br&guild_id=61207059&key=KEY123

### 💬 Exemplo de Resposta
{
  "status": "ok",
  "guildID": "12345678",
  "rodada": 2,
  "data": [
    {
      "player_id": 10000001,
      "pontos": 120
    },
    {
      "player_id": 10000002,
      "pontos": 95
    }
  ]
}

---

## API de Convite para Guilda
Rota da API = https://free-fire-data.vercel.app/api/inviteclanmember?region={region}&guild_id={guild_id}&player_id={player_id}&key={key}

**Endpoint:** `api/inviteclanmember`  
**Método:** `GET`  

Este endpoint envia um convite de entrada na guilda para um jogador.

### 📨 Exemplo de Requisição
GET https://free-fire-data.vercel.app/api/inviteclanmember?region=br&guild_id=61207059&player_id=10000001&key=KEY123

### 💬 Resposta
200 OK → Convite enviado com sucesso

---

## API de Remoção de Membro da Guilda
Rota da API = https://free-fire-data.vercel.app/api/removeclanmember?region={region}&guild_id={guild_id}&player_id={player_id}&key={key}

**Endpoint:** `api/removeclanmember`  
**Método:** `GET`  

Este endpoint remove um jogador da guilda.

### 📨 Exemplo de Requisição
GET https://free-fire-data.vercel.app/api/removeclanmember?region=br&guild_id=61207059&player_id=10000001&key=KEY123

### 💬 Resposta
200 OK → Jogador removido com sucesso


📚 **Objetivo da API**

O objetivo principal de fornecer esta API gratuita é melhorar a experiência da comunidade Free Fire. A Garena Free Fire não oferece APIs oficiais de informações de conta, então esta solução personalizada visa preencher essa lacuna, fornecendo aos jogadores e desenvolvedores dados valiosos da conta.

🧩 **(Alguns dos🤫) Frameworks e Bibliotecas Utilizados**  
- **Flask**: Um micro framework web para Python para construir os endpoints da API.  
- **Flask-CORS**: Para lidar com o Compartilhamento de Recursos entre Origens (CORS).  
- **PyCryptodome**: Para implementar descriptografia e criptografia.  
- **Requests**: Para fazer requisições HTTP ao servidor.

# 📁 Informações Adicionais

- Esta resposta da API não representa a estrutura real recebida do servidor oficial da Garena.  
- A estrutura da resposta é simplificada em um formato amigável para facilitar a compreensão de qualquer pessoa, em qualquer nível de programação.

# 😵 Respostas de Erro
A API pode exibir respostas de erro devido a requisições imprecisas dos usuários!

### Instâncias de Erro e Soluções

- **Código de Erro:**  Havana
  - **Mensagem:** Região inválida.  
  - **Solução:** Certifique-se de estar usando um código de região válido.

- **Código de Erro:** 429
  - **Mensagem:** Requisições anormais detectadas. Evite usar indevidamente a API de Informações para Visitas ou seu IP pode ser bloqueado!  
  - **Solução:** Evite requisições excessivas ou entre em contato com o provedor da API para assistência.

- **Código de Erro:** 500
  - **Mensagem:** Ocorreu um erro ao processar sua requisição. Verifique novamente seu ID e Região.  
  - **Solução:** Verifique novamente o ID de usuário e a região fornecidos e tente novamente a requisição. Se o problema persistir, entre em contato com o provedor da API para suporte.

---

API criada por CebolinhaWiz,  
Todos os direitos reservados!
