shader中声明cubemap

```
_BaseCubeMap("Cube Map", CUBE) = "white" {}
```

hlsl中声明cubemap

```
TextureCube<float4> _CubeMap;
SamplerState sampler_CubeMap;
```

采样cubemap

```
_BaseCubeMap.Sample(sampler_BaseCubeMap, direction);
```

