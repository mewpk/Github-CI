kubectl -n default get secret argocd-initial-admin-secret `
-o jsonpath=
"{.data.password}" | `
% { [Text.Encoding]::UTF8.GetString([Convert]::FromBase64String($_)) }
