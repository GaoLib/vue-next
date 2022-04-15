# 初始化
### packages\runtime-dom\src\index.ts
- createApp
- ensureRenderer().createApp()
- createRenderer()

### packages\runtime-core\src\renderer.ts
- baseCreateRenderer()
- createAppAPI(render, hydrate)

### packages\runtime-core\src\apiCreateApp.ts
- vue 中 app.mount() 执行
- createApp中执行传入的render

### packages\runtime-core\src\renderer.ts
- render()
- patch()
- processComponent()
- mountComponent()
- setupComponent()

### packages\runtime-core\src\component.ts
- initProps()、initSlots()...

### packages\runtime-core\src\renderer.ts
- setupRenderEffect()