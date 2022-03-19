# CadZinho Flatpak

This is an attempt to package [CadZinho](https://github.com/zecruel/CadZinho) into a [Flatpak](https://flatpak.org/).

The most valuable parts are borrowed from other Flatpaks published in Flathub:

- Lua from [com.corsixth.corsixth](https://github.com/flathub/com.corsixth.corsixth/blob/4e67cf632857aa2ddbea93966cc589a9be2f85a1/com.corsixth.corsixth.yml#L24)
- SDL2 from [org.openttd.OpenTTD](https://github.com/flathub/org.openttd.OpenTTD/blob/f4d2e96ead03d099ec6a13f9f0affb82aa64ed50/org.openttd.OpenTTD.yaml#L17)
- glu and glew from [org.kde.krita](https://github.com/flathub/org.kde.krita/blob/ec3f211c56a435bef25f68082fa846bf7f321618/org.kde.krita.yaml#L350)

## Building and running

```
flatpak install flathub org.freedesktop.Platform//21.08 org.freedesktop.Sdk//21.08
flatpak-builder --user --install build-dir org.cadzinho.CadZinho.yml
flatpak run org.cadzinho.CadZinho
```

