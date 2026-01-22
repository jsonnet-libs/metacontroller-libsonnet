---
permalink: /4.12/metacontroller/v1alpha1/compositeController/
---

# metacontroller.v1alpha1.compositeController

"CompositeController"

## Index

* [`fn new(name)`](#fn-new)
* [`obj metadata`](#obj-metadata)
  * [`fn withAnnotations(annotations)`](#fn-metadatawithannotations)
  * [`fn withAnnotationsMixin(annotations)`](#fn-metadatawithannotationsmixin)
  * [`fn withClusterName(clusterName)`](#fn-metadatawithclustername)
  * [`fn withCreationTimestamp(creationTimestamp)`](#fn-metadatawithcreationtimestamp)
  * [`fn withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)`](#fn-metadatawithdeletiongraceperiodseconds)
  * [`fn withDeletionTimestamp(deletionTimestamp)`](#fn-metadatawithdeletiontimestamp)
  * [`fn withFinalizers(finalizers)`](#fn-metadatawithfinalizers)
  * [`fn withFinalizersMixin(finalizers)`](#fn-metadatawithfinalizersmixin)
  * [`fn withGenerateName(generateName)`](#fn-metadatawithgeneratename)
  * [`fn withGeneration(generation)`](#fn-metadatawithgeneration)
  * [`fn withLabels(labels)`](#fn-metadatawithlabels)
  * [`fn withLabelsMixin(labels)`](#fn-metadatawithlabelsmixin)
  * [`fn withName(name)`](#fn-metadatawithname)
  * [`fn withNamespace(namespace)`](#fn-metadatawithnamespace)
  * [`fn withOwnerReferences(ownerReferences)`](#fn-metadatawithownerreferences)
  * [`fn withOwnerReferencesMixin(ownerReferences)`](#fn-metadatawithownerreferencesmixin)
  * [`fn withResourceVersion(resourceVersion)`](#fn-metadatawithresourceversion)
  * [`fn withSelfLink(selfLink)`](#fn-metadatawithselflink)
  * [`fn withUid(uid)`](#fn-metadatawithuid)
* [`obj spec`](#obj-spec)
  * [`fn withChildResources(childResources)`](#fn-specwithchildresources)
  * [`fn withChildResourcesMixin(childResources)`](#fn-specwithchildresourcesmixin)
  * [`fn withGenerateSelector(generateSelector)`](#fn-specwithgenerateselector)
  * [`fn withResyncPeriodSeconds(resyncPeriodSeconds)`](#fn-specwithresyncperiodseconds)
  * [`obj spec.childResources`](#obj-specchildresources)
    * [`fn withApiVersion(apiVersion)`](#fn-specchildresourceswithapiversion)
    * [`fn withResource(resource)`](#fn-specchildresourceswithresource)
    * [`obj spec.childResources.updateStrategy`](#obj-specchildresourcesupdatestrategy)
      * [`fn withMethod(method)`](#fn-specchildresourcesupdatestrategywithmethod)
      * [`obj spec.childResources.updateStrategy.statusChecks`](#obj-specchildresourcesupdatestrategystatuschecks)
        * [`fn withConditions(conditions)`](#fn-specchildresourcesupdatestrategystatuscheckswithconditions)
        * [`fn withConditionsMixin(conditions)`](#fn-specchildresourcesupdatestrategystatuscheckswithconditionsmixin)
        * [`obj spec.childResources.updateStrategy.statusChecks.conditions`](#obj-specchildresourcesupdatestrategystatuschecksconditions)
          * [`fn withReason(reason)`](#fn-specchildresourcesupdatestrategystatuschecksconditionswithreason)
          * [`fn withType(type)`](#fn-specchildresourcesupdatestrategystatuschecksconditionswithtype)
  * [`obj spec.hooks`](#obj-spechooks)
    * [`obj spec.hooks.customize`](#obj-spechookscustomize)
      * [`fn withVersion(version)`](#fn-spechookscustomizewithversion)
      * [`obj spec.hooks.customize.webhook`](#obj-spechookscustomizewebhook)
        * [`fn withPath(path)`](#fn-spechookscustomizewebhookwithpath)
        * [`fn withResponseUnMarshallMode(responseUnMarshallMode)`](#fn-spechookscustomizewebhookwithresponseunmarshallmode)
        * [`fn withTimeout(timeout)`](#fn-spechookscustomizewebhookwithtimeout)
        * [`fn withUrl(url)`](#fn-spechookscustomizewebhookwithurl)
        * [`obj spec.hooks.customize.webhook.etag`](#obj-spechookscustomizewebhooketag)
          * [`fn withCacheCleanupSeconds(cacheCleanupSeconds)`](#fn-spechookscustomizewebhooketagwithcachecleanupseconds)
          * [`fn withCacheTimeoutSeconds(cacheTimeoutSeconds)`](#fn-spechookscustomizewebhooketagwithcachetimeoutseconds)
          * [`fn withEnabled(enabled)`](#fn-spechookscustomizewebhooketagwithenabled)
        * [`obj spec.hooks.customize.webhook.service`](#obj-spechookscustomizewebhookservice)
          * [`fn withName(name)`](#fn-spechookscustomizewebhookservicewithname)
          * [`fn withNamespace(namespace)`](#fn-spechookscustomizewebhookservicewithnamespace)
          * [`fn withPort(port)`](#fn-spechookscustomizewebhookservicewithport)
          * [`fn withProtocol(protocol)`](#fn-spechookscustomizewebhookservicewithprotocol)
    * [`obj spec.hooks.finalize`](#obj-spechooksfinalize)
      * [`fn withVersion(version)`](#fn-spechooksfinalizewithversion)
      * [`obj spec.hooks.finalize.webhook`](#obj-spechooksfinalizewebhook)
        * [`fn withPath(path)`](#fn-spechooksfinalizewebhookwithpath)
        * [`fn withResponseUnMarshallMode(responseUnMarshallMode)`](#fn-spechooksfinalizewebhookwithresponseunmarshallmode)
        * [`fn withTimeout(timeout)`](#fn-spechooksfinalizewebhookwithtimeout)
        * [`fn withUrl(url)`](#fn-spechooksfinalizewebhookwithurl)
        * [`obj spec.hooks.finalize.webhook.etag`](#obj-spechooksfinalizewebhooketag)
          * [`fn withCacheCleanupSeconds(cacheCleanupSeconds)`](#fn-spechooksfinalizewebhooketagwithcachecleanupseconds)
          * [`fn withCacheTimeoutSeconds(cacheTimeoutSeconds)`](#fn-spechooksfinalizewebhooketagwithcachetimeoutseconds)
          * [`fn withEnabled(enabled)`](#fn-spechooksfinalizewebhooketagwithenabled)
        * [`obj spec.hooks.finalize.webhook.service`](#obj-spechooksfinalizewebhookservice)
          * [`fn withName(name)`](#fn-spechooksfinalizewebhookservicewithname)
          * [`fn withNamespace(namespace)`](#fn-spechooksfinalizewebhookservicewithnamespace)
          * [`fn withPort(port)`](#fn-spechooksfinalizewebhookservicewithport)
          * [`fn withProtocol(protocol)`](#fn-spechooksfinalizewebhookservicewithprotocol)
    * [`obj spec.hooks.postUpdateChild`](#obj-spechookspostupdatechild)
      * [`fn withVersion(version)`](#fn-spechookspostupdatechildwithversion)
      * [`obj spec.hooks.postUpdateChild.webhook`](#obj-spechookspostupdatechildwebhook)
        * [`fn withPath(path)`](#fn-spechookspostupdatechildwebhookwithpath)
        * [`fn withResponseUnMarshallMode(responseUnMarshallMode)`](#fn-spechookspostupdatechildwebhookwithresponseunmarshallmode)
        * [`fn withTimeout(timeout)`](#fn-spechookspostupdatechildwebhookwithtimeout)
        * [`fn withUrl(url)`](#fn-spechookspostupdatechildwebhookwithurl)
        * [`obj spec.hooks.postUpdateChild.webhook.etag`](#obj-spechookspostupdatechildwebhooketag)
          * [`fn withCacheCleanupSeconds(cacheCleanupSeconds)`](#fn-spechookspostupdatechildwebhooketagwithcachecleanupseconds)
          * [`fn withCacheTimeoutSeconds(cacheTimeoutSeconds)`](#fn-spechookspostupdatechildwebhooketagwithcachetimeoutseconds)
          * [`fn withEnabled(enabled)`](#fn-spechookspostupdatechildwebhooketagwithenabled)
        * [`obj spec.hooks.postUpdateChild.webhook.service`](#obj-spechookspostupdatechildwebhookservice)
          * [`fn withName(name)`](#fn-spechookspostupdatechildwebhookservicewithname)
          * [`fn withNamespace(namespace)`](#fn-spechookspostupdatechildwebhookservicewithnamespace)
          * [`fn withPort(port)`](#fn-spechookspostupdatechildwebhookservicewithport)
          * [`fn withProtocol(protocol)`](#fn-spechookspostupdatechildwebhookservicewithprotocol)
    * [`obj spec.hooks.preUpdateChild`](#obj-spechookspreupdatechild)
      * [`fn withVersion(version)`](#fn-spechookspreupdatechildwithversion)
      * [`obj spec.hooks.preUpdateChild.webhook`](#obj-spechookspreupdatechildwebhook)
        * [`fn withPath(path)`](#fn-spechookspreupdatechildwebhookwithpath)
        * [`fn withResponseUnMarshallMode(responseUnMarshallMode)`](#fn-spechookspreupdatechildwebhookwithresponseunmarshallmode)
        * [`fn withTimeout(timeout)`](#fn-spechookspreupdatechildwebhookwithtimeout)
        * [`fn withUrl(url)`](#fn-spechookspreupdatechildwebhookwithurl)
        * [`obj spec.hooks.preUpdateChild.webhook.etag`](#obj-spechookspreupdatechildwebhooketag)
          * [`fn withCacheCleanupSeconds(cacheCleanupSeconds)`](#fn-spechookspreupdatechildwebhooketagwithcachecleanupseconds)
          * [`fn withCacheTimeoutSeconds(cacheTimeoutSeconds)`](#fn-spechookspreupdatechildwebhooketagwithcachetimeoutseconds)
          * [`fn withEnabled(enabled)`](#fn-spechookspreupdatechildwebhooketagwithenabled)
        * [`obj spec.hooks.preUpdateChild.webhook.service`](#obj-spechookspreupdatechildwebhookservice)
          * [`fn withName(name)`](#fn-spechookspreupdatechildwebhookservicewithname)
          * [`fn withNamespace(namespace)`](#fn-spechookspreupdatechildwebhookservicewithnamespace)
          * [`fn withPort(port)`](#fn-spechookspreupdatechildwebhookservicewithport)
          * [`fn withProtocol(protocol)`](#fn-spechookspreupdatechildwebhookservicewithprotocol)
    * [`obj spec.hooks.sync`](#obj-spechookssync)
      * [`fn withVersion(version)`](#fn-spechookssyncwithversion)
      * [`obj spec.hooks.sync.webhook`](#obj-spechookssyncwebhook)
        * [`fn withPath(path)`](#fn-spechookssyncwebhookwithpath)
        * [`fn withResponseUnMarshallMode(responseUnMarshallMode)`](#fn-spechookssyncwebhookwithresponseunmarshallmode)
        * [`fn withTimeout(timeout)`](#fn-spechookssyncwebhookwithtimeout)
        * [`fn withUrl(url)`](#fn-spechookssyncwebhookwithurl)
        * [`obj spec.hooks.sync.webhook.etag`](#obj-spechookssyncwebhooketag)
          * [`fn withCacheCleanupSeconds(cacheCleanupSeconds)`](#fn-spechookssyncwebhooketagwithcachecleanupseconds)
          * [`fn withCacheTimeoutSeconds(cacheTimeoutSeconds)`](#fn-spechookssyncwebhooketagwithcachetimeoutseconds)
          * [`fn withEnabled(enabled)`](#fn-spechookssyncwebhooketagwithenabled)
        * [`obj spec.hooks.sync.webhook.service`](#obj-spechookssyncwebhookservice)
          * [`fn withName(name)`](#fn-spechookssyncwebhookservicewithname)
          * [`fn withNamespace(namespace)`](#fn-spechookssyncwebhookservicewithnamespace)
          * [`fn withPort(port)`](#fn-spechookssyncwebhookservicewithport)
          * [`fn withProtocol(protocol)`](#fn-spechookssyncwebhookservicewithprotocol)
  * [`obj spec.parentResource`](#obj-specparentresource)
    * [`fn withApiVersion(apiVersion)`](#fn-specparentresourcewithapiversion)
    * [`fn withIgnoreStatusChanges(ignoreStatusChanges)`](#fn-specparentresourcewithignorestatuschanges)
    * [`fn withResource(resource)`](#fn-specparentresourcewithresource)
    * [`obj spec.parentResource.labelSelector`](#obj-specparentresourcelabelselector)
      * [`fn withMatchExpressions(matchExpressions)`](#fn-specparentresourcelabelselectorwithmatchexpressions)
      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specparentresourcelabelselectorwithmatchexpressionsmixin)
      * [`fn withMatchLabels(matchLabels)`](#fn-specparentresourcelabelselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specparentresourcelabelselectorwithmatchlabelsmixin)
      * [`obj spec.parentResource.labelSelector.matchExpressions`](#obj-specparentresourcelabelselectormatchexpressions)
        * [`fn withKey(key)`](#fn-specparentresourcelabelselectormatchexpressionswithkey)
        * [`fn withOperator(operator)`](#fn-specparentresourcelabelselectormatchexpressionswithoperator)
        * [`fn withValues(values)`](#fn-specparentresourcelabelselectormatchexpressionswithvalues)
        * [`fn withValuesMixin(values)`](#fn-specparentresourcelabelselectormatchexpressionswithvaluesmixin)
    * [`obj spec.parentResource.revisionHistory`](#obj-specparentresourcerevisionhistory)
      * [`fn withFieldPaths(fieldPaths)`](#fn-specparentresourcerevisionhistorywithfieldpaths)
      * [`fn withFieldPathsMixin(fieldPaths)`](#fn-specparentresourcerevisionhistorywithfieldpathsmixin)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of CompositeController

## obj metadata

"ObjectMeta is metadata that all persisted resources must have, which includes all objects users must create."

### fn metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

### fn metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

**Note:** This function appends passed data to existing values

### fn metadata.withClusterName

```ts
withClusterName(clusterName)
```

"The name of the cluster which the object belongs to. This is used to distinguish resources with same name and namespace in different clusters. This field is not set anywhere right now and apiserver is going to ignore it if set in create or update request."

### fn metadata.withCreationTimestamp

```ts
withCreationTimestamp(creationTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withDeletionGracePeriodSeconds

```ts
withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)
```

"Number of seconds allowed for this object to gracefully terminate before it will be removed from the system. Only set when deletionTimestamp is also set. May only be shortened. Read-only."

### fn metadata.withDeletionTimestamp

```ts
withDeletionTimestamp(deletionTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withFinalizers

```ts
withFinalizers(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

### fn metadata.withFinalizersMixin

```ts
withFinalizersMixin(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

**Note:** This function appends passed data to existing values

### fn metadata.withGenerateName

```ts
withGenerateName(generateName)
```

"GenerateName is an optional prefix, used by the server, to generate a unique name ONLY IF the Name field has not been provided. If this field is used, the name returned to the client will be different than the name passed. This value will also be combined with a unique suffix. The provided value has the same validation rules as the Name field, and may be truncated by the length of the suffix required to make the value unique on the server.\n\nIf this field is specified and the generated name exists, the server will NOT return a 409 - instead, it will either return 201 Created or 500 with Reason ServerTimeout indicating a unique name could not be found in the time allotted, and the client should retry (optionally after the time indicated in the Retry-After header).\n\nApplied only if Name is not specified. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency"

### fn metadata.withGeneration

```ts
withGeneration(generation)
```

"A sequence number representing a specific generation of the desired state. Populated by the system. Read-only."

### fn metadata.withLabels

```ts
withLabels(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

### fn metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

**Note:** This function appends passed data to existing values

### fn metadata.withName

```ts
withName(name)
```

"Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/identifiers#names"

### fn metadata.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the space within which each name must be unique. An empty namespace is equivalent to the \"default\" namespace, but \"default\" is the canonical representation. Not all objects are required to be scoped to a namespace - the value of this field for those objects will be empty.\n\nMust be a DNS_LABEL. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/namespaces"

### fn metadata.withOwnerReferences

```ts
withOwnerReferences(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

### fn metadata.withOwnerReferencesMixin

```ts
withOwnerReferencesMixin(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

**Note:** This function appends passed data to existing values

### fn metadata.withResourceVersion

```ts
withResourceVersion(resourceVersion)
```

"An opaque value that represents the internal version of this object that can be used by clients to determine when objects have changed. May be used for optimistic concurrency, change detection, and the watch operation on a resource or set of resources. Clients must treat these values as opaque and passed unmodified back to the server. They may only be valid for a particular resource or set of resources.\n\nPopulated by the system. Read-only. Value must be treated as opaque by clients and . More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency"

### fn metadata.withSelfLink

```ts
withSelfLink(selfLink)
```

"SelfLink is a URL representing this object. Populated by the system. Read-only.\n\nDEPRECATED Kubernetes will stop propagating this field in 1.20 release and the field is planned to be removed in 1.21 release."

### fn metadata.withUid

```ts
withUid(uid)
```

"UID is the unique in time and space value for this object. It is typically generated by the server on successful creation of a resource and is not allowed to change on PUT operations.\n\nPopulated by the system. Read-only. More info: http://kubernetes.io/docs/user-guide/identifiers#uids"

## obj spec



### fn spec.withChildResources

```ts
withChildResources(childResources)
```



### fn spec.withChildResourcesMixin

```ts
withChildResourcesMixin(childResources)
```



**Note:** This function appends passed data to existing values

### fn spec.withGenerateSelector

```ts
withGenerateSelector(generateSelector)
```



### fn spec.withResyncPeriodSeconds

```ts
withResyncPeriodSeconds(resyncPeriodSeconds)
```



## obj spec.childResources



### fn spec.childResources.withApiVersion

```ts
withApiVersion(apiVersion)
```



### fn spec.childResources.withResource

```ts
withResource(resource)
```



## obj spec.childResources.updateStrategy



### fn spec.childResources.updateStrategy.withMethod

```ts
withMethod(method)
```



## obj spec.childResources.updateStrategy.statusChecks



### fn spec.childResources.updateStrategy.statusChecks.withConditions

```ts
withConditions(conditions)
```



### fn spec.childResources.updateStrategy.statusChecks.withConditionsMixin

```ts
withConditionsMixin(conditions)
```



**Note:** This function appends passed data to existing values

## obj spec.childResources.updateStrategy.statusChecks.conditions



### fn spec.childResources.updateStrategy.statusChecks.conditions.withReason

```ts
withReason(reason)
```



### fn spec.childResources.updateStrategy.statusChecks.conditions.withType

```ts
withType(type)
```



## obj spec.hooks



## obj spec.hooks.customize



### fn spec.hooks.customize.withVersion

```ts
withVersion(version)
```



## obj spec.hooks.customize.webhook



### fn spec.hooks.customize.webhook.withPath

```ts
withPath(path)
```



### fn spec.hooks.customize.webhook.withResponseUnMarshallMode

```ts
withResponseUnMarshallMode(responseUnMarshallMode)
```

"Sets the json unmarshall mode. One of the 'loose' or 'strict'. In 'strict'\nmode additional checks are performed to detect unknown and duplicated fields."

### fn spec.hooks.customize.webhook.withTimeout

```ts
withTimeout(timeout)
```



### fn spec.hooks.customize.webhook.withUrl

```ts
withUrl(url)
```



## obj spec.hooks.customize.webhook.etag



### fn spec.hooks.customize.webhook.etag.withCacheCleanupSeconds

```ts
withCacheCleanupSeconds(cacheCleanupSeconds)
```



### fn spec.hooks.customize.webhook.etag.withCacheTimeoutSeconds

```ts
withCacheTimeoutSeconds(cacheTimeoutSeconds)
```



### fn spec.hooks.customize.webhook.etag.withEnabled

```ts
withEnabled(enabled)
```



## obj spec.hooks.customize.webhook.service



### fn spec.hooks.customize.webhook.service.withName

```ts
withName(name)
```



### fn spec.hooks.customize.webhook.service.withNamespace

```ts
withNamespace(namespace)
```



### fn spec.hooks.customize.webhook.service.withPort

```ts
withPort(port)
```



### fn spec.hooks.customize.webhook.service.withProtocol

```ts
withProtocol(protocol)
```



## obj spec.hooks.finalize



### fn spec.hooks.finalize.withVersion

```ts
withVersion(version)
```



## obj spec.hooks.finalize.webhook



### fn spec.hooks.finalize.webhook.withPath

```ts
withPath(path)
```



### fn spec.hooks.finalize.webhook.withResponseUnMarshallMode

```ts
withResponseUnMarshallMode(responseUnMarshallMode)
```

"Sets the json unmarshall mode. One of the 'loose' or 'strict'. In 'strict'\nmode additional checks are performed to detect unknown and duplicated fields."

### fn spec.hooks.finalize.webhook.withTimeout

```ts
withTimeout(timeout)
```



### fn spec.hooks.finalize.webhook.withUrl

```ts
withUrl(url)
```



## obj spec.hooks.finalize.webhook.etag



### fn spec.hooks.finalize.webhook.etag.withCacheCleanupSeconds

```ts
withCacheCleanupSeconds(cacheCleanupSeconds)
```



### fn spec.hooks.finalize.webhook.etag.withCacheTimeoutSeconds

```ts
withCacheTimeoutSeconds(cacheTimeoutSeconds)
```



### fn spec.hooks.finalize.webhook.etag.withEnabled

```ts
withEnabled(enabled)
```



## obj spec.hooks.finalize.webhook.service



### fn spec.hooks.finalize.webhook.service.withName

```ts
withName(name)
```



### fn spec.hooks.finalize.webhook.service.withNamespace

```ts
withNamespace(namespace)
```



### fn spec.hooks.finalize.webhook.service.withPort

```ts
withPort(port)
```



### fn spec.hooks.finalize.webhook.service.withProtocol

```ts
withProtocol(protocol)
```



## obj spec.hooks.postUpdateChild



### fn spec.hooks.postUpdateChild.withVersion

```ts
withVersion(version)
```



## obj spec.hooks.postUpdateChild.webhook



### fn spec.hooks.postUpdateChild.webhook.withPath

```ts
withPath(path)
```



### fn spec.hooks.postUpdateChild.webhook.withResponseUnMarshallMode

```ts
withResponseUnMarshallMode(responseUnMarshallMode)
```

"Sets the json unmarshall mode. One of the 'loose' or 'strict'. In 'strict'\nmode additional checks are performed to detect unknown and duplicated fields."

### fn spec.hooks.postUpdateChild.webhook.withTimeout

```ts
withTimeout(timeout)
```



### fn spec.hooks.postUpdateChild.webhook.withUrl

```ts
withUrl(url)
```



## obj spec.hooks.postUpdateChild.webhook.etag



### fn spec.hooks.postUpdateChild.webhook.etag.withCacheCleanupSeconds

```ts
withCacheCleanupSeconds(cacheCleanupSeconds)
```



### fn spec.hooks.postUpdateChild.webhook.etag.withCacheTimeoutSeconds

```ts
withCacheTimeoutSeconds(cacheTimeoutSeconds)
```



### fn spec.hooks.postUpdateChild.webhook.etag.withEnabled

```ts
withEnabled(enabled)
```



## obj spec.hooks.postUpdateChild.webhook.service



### fn spec.hooks.postUpdateChild.webhook.service.withName

```ts
withName(name)
```



### fn spec.hooks.postUpdateChild.webhook.service.withNamespace

```ts
withNamespace(namespace)
```



### fn spec.hooks.postUpdateChild.webhook.service.withPort

```ts
withPort(port)
```



### fn spec.hooks.postUpdateChild.webhook.service.withProtocol

```ts
withProtocol(protocol)
```



## obj spec.hooks.preUpdateChild



### fn spec.hooks.preUpdateChild.withVersion

```ts
withVersion(version)
```



## obj spec.hooks.preUpdateChild.webhook



### fn spec.hooks.preUpdateChild.webhook.withPath

```ts
withPath(path)
```



### fn spec.hooks.preUpdateChild.webhook.withResponseUnMarshallMode

```ts
withResponseUnMarshallMode(responseUnMarshallMode)
```

"Sets the json unmarshall mode. One of the 'loose' or 'strict'. In 'strict'\nmode additional checks are performed to detect unknown and duplicated fields."

### fn spec.hooks.preUpdateChild.webhook.withTimeout

```ts
withTimeout(timeout)
```



### fn spec.hooks.preUpdateChild.webhook.withUrl

```ts
withUrl(url)
```



## obj spec.hooks.preUpdateChild.webhook.etag



### fn spec.hooks.preUpdateChild.webhook.etag.withCacheCleanupSeconds

```ts
withCacheCleanupSeconds(cacheCleanupSeconds)
```



### fn spec.hooks.preUpdateChild.webhook.etag.withCacheTimeoutSeconds

```ts
withCacheTimeoutSeconds(cacheTimeoutSeconds)
```



### fn spec.hooks.preUpdateChild.webhook.etag.withEnabled

```ts
withEnabled(enabled)
```



## obj spec.hooks.preUpdateChild.webhook.service



### fn spec.hooks.preUpdateChild.webhook.service.withName

```ts
withName(name)
```



### fn spec.hooks.preUpdateChild.webhook.service.withNamespace

```ts
withNamespace(namespace)
```



### fn spec.hooks.preUpdateChild.webhook.service.withPort

```ts
withPort(port)
```



### fn spec.hooks.preUpdateChild.webhook.service.withProtocol

```ts
withProtocol(protocol)
```



## obj spec.hooks.sync



### fn spec.hooks.sync.withVersion

```ts
withVersion(version)
```



## obj spec.hooks.sync.webhook



### fn spec.hooks.sync.webhook.withPath

```ts
withPath(path)
```



### fn spec.hooks.sync.webhook.withResponseUnMarshallMode

```ts
withResponseUnMarshallMode(responseUnMarshallMode)
```

"Sets the json unmarshall mode. One of the 'loose' or 'strict'. In 'strict'\nmode additional checks are performed to detect unknown and duplicated fields."

### fn spec.hooks.sync.webhook.withTimeout

```ts
withTimeout(timeout)
```



### fn spec.hooks.sync.webhook.withUrl

```ts
withUrl(url)
```



## obj spec.hooks.sync.webhook.etag



### fn spec.hooks.sync.webhook.etag.withCacheCleanupSeconds

```ts
withCacheCleanupSeconds(cacheCleanupSeconds)
```



### fn spec.hooks.sync.webhook.etag.withCacheTimeoutSeconds

```ts
withCacheTimeoutSeconds(cacheTimeoutSeconds)
```



### fn spec.hooks.sync.webhook.etag.withEnabled

```ts
withEnabled(enabled)
```



## obj spec.hooks.sync.webhook.service



### fn spec.hooks.sync.webhook.service.withName

```ts
withName(name)
```



### fn spec.hooks.sync.webhook.service.withNamespace

```ts
withNamespace(namespace)
```



### fn spec.hooks.sync.webhook.service.withPort

```ts
withPort(port)
```



### fn spec.hooks.sync.webhook.service.withProtocol

```ts
withProtocol(protocol)
```



## obj spec.parentResource



### fn spec.parentResource.withApiVersion

```ts
withApiVersion(apiVersion)
```



### fn spec.parentResource.withIgnoreStatusChanges

```ts
withIgnoreStatusChanges(ignoreStatusChanges)
```



### fn spec.parentResource.withResource

```ts
withResource(resource)
```



## obj spec.parentResource.labelSelector

"A label selector is a label query over a set of resources. The result of matchLabels and\nmatchExpressions are ANDed. An empty label selector matches all objects. A null\nlabel selector matches no objects."

### fn spec.parentResource.labelSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.parentResource.labelSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.parentResource.labelSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.parentResource.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.parentResource.labelSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.parentResource.labelSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.parentResource.labelSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.parentResource.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

### fn spec.parentResource.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

**Note:** This function appends passed data to existing values

## obj spec.parentResource.revisionHistory



### fn spec.parentResource.revisionHistory.withFieldPaths

```ts
withFieldPaths(fieldPaths)
```



### fn spec.parentResource.revisionHistory.withFieldPathsMixin

```ts
withFieldPathsMixin(fieldPaths)
```



**Note:** This function appends passed data to existing values