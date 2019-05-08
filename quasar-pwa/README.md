# Esse projeto foi construido com [Quasar Framework](https://quasar-framework.org/guide/pwa-configuring-pwa.html).

## Como foi criado

Primeiro instale o vue-cli globalmente:
`npm i vue-cli -g`

Depois instale o quasar-cli globalmente:
`npm i quasar-cli -g`

Crie o projeto com:
`quasar init quasar-pwa`

Depois de criar o projeto e instalar dependencias, habilite o modo pwa do quasar:
`quasar mode -a pwa`

Rode o projeto com:
`quasar dev -m pwa`

No arquivo quasar.conf.js, modifique o script para a seguinte estrutura:

```js
pwa: {
      // workboxPluginMode: 'InjectManifest',
      // workboxOptions: {},
      manifest: {
        name: 'Quasar App',
        short_name: 'Quasar-PWA',
        description: 'Best PWA App in town!',
        display: 'standalone',
        orientation: 'portrait',
        background_color: '#ffffff',
        theme_color: '#027be3',
        icons: [
          {
            'src': 'statics/icons/icon-128x128.png',
            'sizes': '128x128',
            'type': 'image/png'
          },
          {
            'src': 'statics/icons/icon-192x192.png',
            'sizes': '192x192',
            'type': 'image/png'
          },
          {
            'src': 'statics/icons/icon-256x256.png',
            'sizes': '256x256',
            'type': 'image/png'
          },
          {
            'src': 'statics/icons/icon-384x384.png',
            'sizes': '384x384',
            'type': 'image/png'
          },
          {
            'src': 'statics/icons/icon-512x512.png',
            'sizes': '512x512',
            'type': 'image/png'
          }
        ]
      }
    },
```

Agora é só verificar o funcionamento do service worker nas ferramentas de desenvolvedor de seu browser 😃
