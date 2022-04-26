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


# data定义方法
### packages\runtime-core\src\component.ts
- setupComponent()
  处理 data、props、slots

### packages\runtime-core\src\component.ts
- setupStatefulComponent()
  调用setup，得到返回值

### packages\runtime-core\src\component.ts
- handleSetupResult()
  处理setup返回值：函数为render，对象为setupState

### packages\runtime-core\src\component.ts
- finishComponentSetup()
  兼容 vue2 的data写法

### packages\runtime-core\src\component.ts
- applyOptions()
  处理选项