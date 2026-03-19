# testando geração

- em 260319: GEMINI NÃO TEM MAIS GERAÇÃO DE IMAGEM NO PLANO FREE
rodando com node 
```
--env-file=.env gerar-dinos.mjs
```

este modelo da erro de créditos...
```
// const MODEL = "gemini-3.1-flash-image-preview";
```

```
script-criador> node --env-file=.env gerar-dinos.mjs Gerando T-Rex... Erro em T-Rex: {"error":{"code":429,"message":"You exceeded your current quota, please check your plan and billing details. For more information on this error, head to: https://ai.google.dev/gemini-api/docs/rate-limits. To monitor your current usage, head to: https://ai.dev/rate-limit. \n* Quota exceeded for metric: generativelanguage.googleapis.com/generate_content_free_tier_requests, limit: 0, model: gemini-3.1-flash-image\n* Quota exceeded for metric: generativelanguage.googleapis.com/generate_content_free_tier_requests, limit: 0, model: gemini-3.1-flash-image\n* Quota exceeded for metric: generativelanguage.googleapis.com/generate_content_free_tier_input_token_count, limit: 0, model: gemini-3.1-flash-image\nPlease retry in 54.785608351s.","status":"RESOURCE_EXHAUSTED","details":[{"@type":"type.googleapis.com/google.rpc.Help","links":[{"description":"Learn more about Gemini API quotas","url":"https://ai.google.dev/gemini-api/docs/rate-limits"}]},{"@type":"type.googleapis.com/google.rpc.QuotaFailure","violations":[{"quotaMetric":"generativelanguage.googleapis.com/generate_content_free_tier_requests","quotaId":"GenerateRequestsPerDayPerProjectPerModel-FreeTier","quotaDimensions":{"location":"global","model":"gemini-3.1-flash-image"}},{"quotaMetric":"generativelanguage.googleapis.com/generate_content_free_tier_requests","quotaId":"GenerateRequestsPerMinutePerProjectPerModel-FreeTier","quotaDimensions":{"location":"global","model":"gemini-3.1-flash-image"}},{"quotaMetric":"generativelanguage.googleapis.com/generate_content_free_tier_input_token_count","quotaId":"GenerateContentInputTokensPerModelPerMinute-FreeTier","quotaDimensions":{"location":"global","model":"gemini-3.1-flash-image"}}]},{"@type":"type.googleapis.com/google.rpc.RetryInfo","retryDelay":"54s"}]}}
```

Com este o erro é outro
```
const MODEL = "gemini-2.5-flash";
```
```
script-criador> node --env-file=.env gerar-dinos.mjs
Gerando T-Rex...
Erro em T-Rex: A resposta não trouxe imagem.
Gerando Triceratops...
Erro em Triceratops: A resposta não trouxe imagem.
```



