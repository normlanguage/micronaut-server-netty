# micronaut.server.netty Skill

Use this skill to work with Norm module `micronaut.server.netty` version 5. Use only declarations listed below.

## `micronaut.server.netty.context`

Source: `context/ApplicationContextLifeCycle.norm`

### `ApplicationContextLifeCycle`

```norm
interface ApplicationContextLifeCycle<T extends ApplicationContextLifeCycle<T>> extends ApplicationContextProvider, LifeCycle<T>
```

Type parameters:

- `T` extends `ApplicationContextLifeCycle<T>`

#### `close`

```norm
Void close()
```

Returns: `Void`

## `micronaut.server.netty.context`

Source: `context/ApplicationContextProvider.norm`

### `ApplicationContextProvider`

```norm
interface ApplicationContextProvider
```

## `micronaut.server.netty.context`

Source: `context/LifeCycle.norm`

### `LifeCycle`

```norm
interface LifeCycle<T extends LifeCycle<T>> extends Closeable, AutoCloseable
```

Type parameters:

- `T` extends `LifeCycle<T>`

#### `close`

```norm
Void close()
```

Returns: `Void`

## `micronaut.server.netty.context.event`

Source: `context/event/ApplicationEvent.norm`

### `ApplicationEvent`

```norm
class ApplicationEvent extends EventObject implements Serializable
```

#### `ApplicationEvent`

```norm
ApplicationEvent(__JarBindingToken token)
```

Parameters:

- `token`: `__JarBindingToken`

## `micronaut.server.netty.context.event`

Source: `context/event/ApplicationEventListener.norm`

### `ApplicationEventListener`

```norm
interface ApplicationEventListener<E> extends EventListener
```

Type parameters:

- `E`

## `micronaut.server.netty.core.order`

Source: `core/order/Ordered.norm`

### `Ordered`

```norm
interface Ordered
```

## `micronaut.server.netty.http.netty.channel`

Source: `http/netty/channel/ChannelPipelineCustomizer.norm`

### `ChannelPipelineCustomizer`

```norm
interface ChannelPipelineCustomizer
```

## `micronaut.server.netty.http.netty.websocket`

Source: `http/netty/websocket/WebSocketSessionRepository.norm`

### `WebSocketSessionRepository`

```norm
interface WebSocketSessionRepository
```

## `micronaut.server.netty.http.server.netty`

Source: `http/server/netty/NettyEmbeddedServer.norm`

### `NettyEmbeddedServer`

```norm
interface NettyEmbeddedServer extends EmbeddedServer, WebSocketSessionRepository, ChannelPipelineCustomizer, RefreshEventListener, NettyServerCustomizer_Registry, GracefulShutdownCapable
```

#### `close`

```norm
Void close()
```

Returns: `Void`

## `micronaut.server.netty.http.server.netty`

Source: `http/server/netty/NettyServerCustomizer_Registry.norm`

### `NettyServerCustomizer_Registry`

```norm
interface NettyServerCustomizer_Registry
```

## `micronaut.server.netty.runtime`

Source: `runtime/EmbeddedApplication.norm`

### `EmbeddedApplication`

```norm
interface EmbeddedApplication<T extends EmbeddedApplication<T>> extends ApplicationContextLifeCycle<T>
```

Type parameters:

- `T` extends `EmbeddedApplication<T>`

#### `close`

```norm
Void close()
```

Returns: `Void`

## `micronaut.server.netty.runtime.context.scope.refresh`

Source: `runtime/context/scope/refresh/RefreshEvent.norm`

### `RefreshEvent`

```norm
class RefreshEvent extends ApplicationEvent implements Serializable
```

#### `RefreshEvent`

```norm
RefreshEvent(__JarBindingToken token)
```

Parameters:

- `token`: `__JarBindingToken`

## `micronaut.server.netty.runtime.context.scope.refresh`

Source: `runtime/context/scope/refresh/RefreshEventListener.norm`

### `RefreshEventListener`

```norm
interface RefreshEventListener extends ApplicationEventListener<RefreshEvent>, Ordered
```

## `micronaut.server.netty.runtime.graceful`

Source: `runtime/graceful/GracefulShutdownCapable.norm`

### `GracefulShutdownCapable`

```norm
interface GracefulShutdownCapable
```

## `micronaut.server.netty.runtime.server`

Source: `runtime/server/EmbeddedServer.norm`

### `EmbeddedServer`

```norm
interface EmbeddedServer extends EmbeddedApplication<EmbeddedServer>
```

#### `close`

```norm
Void close()
```

Returns: `Void`

