- 虚拟环境 base url: <http://10.60.38.173:5525>

- 物理环境 base url: <http://10.60.38.173:5530>



#### tool/api/v1.0/get_namespace

```json
{
    "detail": {
        "10.60.38.181": {
            "_ansible_no_log": false,
            "_ansible_parsed": true,
            "changed": false,
            "invocation": {
                "module_args": {
                    "api_key": null,
                    "api_version": "v1",
                    "cert_file": null,
                    "context": null,
                    "field_selectors": [],
                    "host": null,
                    "key_file": null,
                    "kind": "namespace",
                    "kubeconfig": null,
                    "label_selectors": [],
                    "name": null,
                    "namespace": null,
                    "password": null,
                    "ssl_ca_cert": null,
                    "username": null,
                    "verify_ssl": null
                }
            },
            "resources": [
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:28:37Z",
                        "name": "default",
                        "resourceVersion": "4",
                        "selfLink": "/api/v1/namespaces/default",
                        "uid": "18ac482a-55e2-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "finalizers": [
                            "kubernetes"
                        ]
                    },
                    "status": {
                        "phase": "Active"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:28:38Z",
                        "name": "kube-public",
                        "resourceVersion": "37",
                        "selfLink": "/api/v1/namespaces/kube-public",
                        "uid": "190ecba4-55e2-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "finalizers": [
                            "kubernetes"
                        ]
                    },
                    "status": {
                        "phase": "Active"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:28:38Z",
                        "name": "kube-system",
                        "resourceVersion": "36",
                        "selfLink": "/api/v1/namespaces/kube-system",
                        "uid": "19096d86-55e2-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "finalizers": [
                            "kubernetes"
                        ]
                    },
                    "status": {
                        "phase": "Active"
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Namespace\",\"metadata\":{\"annotations\":{},\"name\":\"monitoring\"}}\n"
                        },
                        "creationTimestamp": "2019-04-04T08:51:31Z",
                        "name": "monitoring",
                        "resourceVersion": "147396",
                        "selfLink": "/api/v1/namespaces/monitoring",
                        "uid": "d8002538-56b6-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "finalizers": [
                            "kubernetes"
                        ]
                    },
                    "status": {
                        "phase": "Active"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:36Z",
                        "name": "sock-shop",
                        "resourceVersion": "1131",
                        "selfLink": "/api/v1/namespaces/sock-shop",
                        "uid": "1209c83d-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "finalizers": [
                            "kubernetes"
                        ]
                    },
                    "status": {
                        "phase": "Active"
                    }
                }
            ]
        }
    },
    "failed": {},
    "skipped": {},
    "status": {},
    "success": [
        {
            "creationTimestamp": "2019-04-03T07:28:37Z",
            "name": "default",
            "uid": "18ac482a-55e2-11e9-a74e-002481eeda4c"
        },
        {
            "creationTimestamp": "2019-04-03T07:28:38Z",
            "name": "kube-public",
            "uid": "190ecba4-55e2-11e9-a74e-002481eeda4c"
        },
        {
            "creationTimestamp": "2019-04-03T07:28:38Z",
            "name": "kube-system",
            "uid": "19096d86-55e2-11e9-a74e-002481eeda4c"
        },
        {
            "creationTimestamp": "2019-04-04T08:51:31Z",
            "name": "monitoring",
            "uid": "d8002538-56b6-11e9-a74e-002481eeda4c"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:36Z",
            "name": "sock-shop",
            "uid": "1209c83d-55e3-11e9-a74e-002481eeda4c"
        }
    ],
    "unreachable": {}
}
```

####  tool/api/v1.0/get_pods/sock-shop

```json
{
    "detail": {
        "10.60.38.181": {
            "_ansible_no_log": false,
            "_ansible_parsed": true,
            "changed": false,
            "invocation": {
                "module_args": {
                    "api_key": null,
                    "api_version": "v1",
                    "cert_file": null,
                    "context": null,
                    "field_selectors": [],
                    "host": null,
                    "key_file": null,
                    "kind": "Pod",
                    "kubeconfig": null,
                    "label_selectors": [],
                    "name": null,
                    "namespace": "sock-shop",
                    "password": null,
                    "ssl_ca_cert": null,
                    "username": null,
                    "verify_ssl": null
                }
            },
            "resources": [
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:48Z",
                        "generateName": "carts-648d5f498d-",
                        "labels": {
                            "name": "carts",
                            "pod-template-hash": "648d5f498d"
                        },
                        "name": "carts-648d5f498d-tgq2k",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "carts-648d5f498d",
                                "uid": "19364acf-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "1486",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/carts-648d5f498d-tgq2k",
                        "uid": "193b748b-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "env": [
                                    {
                                        "name": "ZIPKIN",
                                        "value": "zipkin.jaeger.svc.cluster.local"
                                    },
                                    {
                                        "name": "JAVA_OPTS",
                                        "value": "-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom"
                                    }
                                ],
                                "image": "weaveworksdemos/carts:0.4.8",
                                "imagePullPolicy": "IfNotPresent",
                                "name": "carts",
                                "ports": [
                                    {
                                        "containerPort": 80,
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "securityContext": {
                                    "capabilities": {
                                        "add": [
                                            "NET_BIND_SERVICE"
                                        ],
                                        "drop": [
                                            "all"
                                        ]
                                    },
                                    "procMount": "Default",
                                    "readOnlyRootFilesystem": true,
                                    "runAsNonRoot": true,
                                    "runAsUser": 10001
                                },
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/tmp",
                                        "name": "tmp-volume"
                                    },
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.206",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "emptyDir": {
                                    "medium": "Memory"
                                },
                                "name": "tmp-volume"
                            },
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:48Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:36:56Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:36:56Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:48Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://aeafd16d421bf96ecdb6b16fabecc48ec3ecb1eb69857d46355dd6df9706e3c0",
                                "image": "weaveworksdemos/carts:0.4.8",
                                "imageID": "docker-pullable://weaveworksdemos/carts@sha256:434d2f5a6e0e8beef1f253fe96f45b8437a703125fc003434c5282ecf8969a4f",
                                "lastState": {},
                                "name": "carts",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:36:55Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.206",
                        "phase": "Running",
                        "podIP": "172.20.3.4",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:48Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:47Z",
                        "generateName": "carts-db-64b6cc584f-",
                        "labels": {
                            "name": "carts-db",
                            "pod-template-hash": "64b6cc584f"
                        },
                        "name": "carts-db-64b6cc584f-6tbvj",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "carts-db-64b6cc584f",
                                "uid": "1900b8a7-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "1624",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/carts-db-64b6cc584f-6tbvj",
                        "uid": "1905297e-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "image": "mongo",
                                "imagePullPolicy": "Always",
                                "name": "carts-db",
                                "ports": [
                                    {
                                        "containerPort": 27017,
                                        "name": "mongo",
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "securityContext": {
                                    "capabilities": {
                                        "add": [
                                            "CHOWN",
                                            "SETGID",
                                            "SETUID"
                                        ],
                                        "drop": [
                                            "all"
                                        ]
                                    },
                                    "procMount": "Default",
                                    "readOnlyRootFilesystem": true
                                },
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/tmp",
                                        "name": "tmp-volume"
                                    },
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.133",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "emptyDir": {
                                    "medium": "Memory"
                                },
                                "name": "tmp-volume"
                            },
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:47Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:38:10Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:38:10Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:47Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://3e30be7ada96d22e9e914fc44f6fe8f66c45eb2f294a92affb17cff689f92644",
                                "image": "mongo:latest",
                                "imageID": "docker-pullable://mongo@sha256:f025ed224f93086ce4ddc8f61a4aa8113e8dcd6106ca0e3a599f9a0d76ab94ad",
                                "lastState": {},
                                "name": "carts-db",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:38:10Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.133",
                        "phase": "Running",
                        "podIP": "172.20.2.2",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:47Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:49Z",
                        "generateName": "catalogue-6759fc9bf5-",
                        "labels": {
                            "name": "catalogue",
                            "pod-template-hash": "6759fc9bf5"
                        },
                        "name": "catalogue-6759fc9bf5-9nfjb",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "catalogue-6759fc9bf5",
                                "uid": "19c3bc18-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "1546",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/catalogue-6759fc9bf5-9nfjb",
                        "uid": "19c91d2e-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "image": "weaveworksdemos/catalogue:0.3.5",
                                "imagePullPolicy": "IfNotPresent",
                                "name": "catalogue",
                                "ports": [
                                    {
                                        "containerPort": 80,
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "securityContext": {
                                    "capabilities": {
                                        "add": [
                                            "NET_BIND_SERVICE"
                                        ],
                                        "drop": [
                                            "all"
                                        ]
                                    },
                                    "procMount": "Default",
                                    "readOnlyRootFilesystem": true,
                                    "runAsNonRoot": true,
                                    "runAsUser": 10001
                                },
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.188",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:49Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:37:31Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:37:31Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:49Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://2b7e3465e9681185387fcbb92aef2bee9d2aeff60e94e969acd2f9f52b03dd59",
                                "image": "weaveworksdemos/catalogue:0.3.5",
                                "imageID": "docker-pullable://weaveworksdemos/catalogue@sha256:0147a65b7116569439eefb1a6dbed455fe022464ef70e0c3cab75bc4a226b39b",
                                "lastState": {},
                                "name": "catalogue",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:37:31Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.188",
                        "phase": "Running",
                        "podIP": "172.20.4.3",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:49Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:48Z",
                        "generateName": "catalogue-db-99cbcbb88-",
                        "labels": {
                            "name": "catalogue-db",
                            "pod-template-hash": "99cbcbb88"
                        },
                        "name": "catalogue-db-99cbcbb88-8wdp5",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "catalogue-db-99cbcbb88",
                                "uid": "19849165-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "1837",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/catalogue-db-99cbcbb88-8wdp5",
                        "uid": "1985a47a-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "env": [
                                    {
                                        "name": "MYSQL_ROOT_PASSWORD",
                                        "value": "fake_password"
                                    },
                                    {
                                        "name": "MYSQL_DATABASE",
                                        "value": "socksdb"
                                    }
                                ],
                                "image": "weaveworksdemos/catalogue-db:0.3.0",
                                "imagePullPolicy": "IfNotPresent",
                                "name": "catalogue-db",
                                "ports": [
                                    {
                                        "containerPort": 3306,
                                        "name": "mysql",
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.133",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:48Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:40:03Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:40:03Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:48Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://269ebcf6e77cdb719caf1949990b1869d9a09b11fcb0321d50af90c8c0086cf2",
                                "image": "weaveworksdemos/catalogue-db:0.3.0",
                                "imageID": "docker-pullable://weaveworksdemos/catalogue-db@sha256:7ba74ec9adf88f6625b8d85d3323d1ee5232b39877e1590021ea485cf9457251",
                                "lastState": {},
                                "name": "catalogue-db",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:40:02Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.133",
                        "phase": "Running",
                        "podIP": "172.20.2.3",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:48Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:49Z",
                        "generateName": "front-end-77b48955b6-",
                        "labels": {
                            "name": "front-end",
                            "pod-template-hash": "77b48955b6"
                        },
                        "name": "front-end-77b48955b6-spjsh",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "front-end-77b48955b6",
                                "uid": "19f1c2c3-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "1577",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/front-end-77b48955b6-spjsh",
                        "uid": "19f750a9-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "image": "weaveworksdemos/front-end:0.3.12",
                                "imagePullPolicy": "IfNotPresent",
                                "name": "front-end",
                                "ports": [
                                    {
                                        "containerPort": 8079,
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {
                                    "requests": {
                                        "cpu": "100m",
                                        "memory": "100Mi"
                                    }
                                },
                                "securityContext": {
                                    "capabilities": {
                                        "drop": [
                                            "all"
                                        ]
                                    },
                                    "procMount": "Default",
                                    "readOnlyRootFilesystem": true,
                                    "runAsNonRoot": true,
                                    "runAsUser": 10001
                                },
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.205",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:49Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:37:43Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:37:43Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:49Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://c71f3095201d6f8a58f3357d423c33414fa6a635239d7d5af908ccf787839acf",
                                "image": "weaveworksdemos/front-end:0.3.12",
                                "imageID": "docker-pullable://weaveworksdemos/front-end@sha256:26a2d9b6b291dee2dca32fca3f5bff6c2fa07bb5954359afcbc8001cc70eac71",
                                "lastState": {},
                                "name": "front-end",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:37:42Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.205",
                        "phase": "Running",
                        "podIP": "172.20.1.4",
                        "qosClass": "Burstable",
                        "startTime": "2019-04-03T07:35:49Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:50Z",
                        "generateName": "orders-6496fcd6f7-",
                        "labels": {
                            "name": "orders",
                            "pod-template-hash": "6496fcd6f7"
                        },
                        "name": "orders-6496fcd6f7-rz24g",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "orders-6496fcd6f7",
                                "uid": "1a61d026-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "1756",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/orders-6496fcd6f7-rz24g",
                        "uid": "1a633f87-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "env": [
                                    {
                                        "name": "ZIPKIN",
                                        "value": "zipkin.jaeger.svc.cluster.local"
                                    },
                                    {
                                        "name": "JAVA_OPTS",
                                        "value": "-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom"
                                    }
                                ],
                                "image": "weaveworksdemos/orders:0.4.7",
                                "imagePullPolicy": "IfNotPresent",
                                "name": "orders",
                                "ports": [
                                    {
                                        "containerPort": 80,
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "securityContext": {
                                    "capabilities": {
                                        "add": [
                                            "NET_BIND_SERVICE"
                                        ],
                                        "drop": [
                                            "all"
                                        ]
                                    },
                                    "procMount": "Default",
                                    "readOnlyRootFilesystem": true,
                                    "runAsNonRoot": true,
                                    "runAsUser": 10001
                                },
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/tmp",
                                        "name": "tmp-volume"
                                    },
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.188",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "emptyDir": {
                                    "medium": "Memory"
                                },
                                "name": "tmp-volume"
                            },
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:50Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:39:18Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:39:18Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:50Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://016d5fcee0ca35aac078d7c5543143e19f65ac01d34265ea93ddac83748cd2d6",
                                "image": "weaveworksdemos/orders:0.4.7",
                                "imageID": "docker-pullable://weaveworksdemos/orders@sha256:b622e40e83433baf6374f15e076b53893f79958640fc6667dff597622eff03b9",
                                "lastState": {},
                                "name": "orders",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:39:18Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.188",
                        "phase": "Running",
                        "podIP": "172.20.4.4",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:50Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:49Z",
                        "generateName": "orders-db-86f5c494b9-",
                        "labels": {
                            "name": "orders-db",
                            "pod-template-hash": "86f5c494b9"
                        },
                        "name": "orders-db-86f5c494b9-v8fkr",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "orders-db-86f5c494b9",
                                "uid": "1a3a0f11-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "1933",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/orders-db-86f5c494b9-v8fkr",
                        "uid": "1a3aa497-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "image": "mongo",
                                "imagePullPolicy": "Always",
                                "name": "orders-db",
                                "ports": [
                                    {
                                        "containerPort": 27017,
                                        "name": "mongo",
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "securityContext": {
                                    "capabilities": {
                                        "add": [
                                            "CHOWN",
                                            "SETGID",
                                            "SETUID"
                                        ],
                                        "drop": [
                                            "all"
                                        ]
                                    },
                                    "procMount": "Default",
                                    "readOnlyRootFilesystem": true
                                },
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/tmp",
                                        "name": "tmp-volume"
                                    },
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.133",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "emptyDir": {
                                    "medium": "Memory"
                                },
                                "name": "tmp-volume"
                            },
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:50Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:40:55Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:40:55Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:49Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://50b6ed8a4e8e5671978bdcbd01bbbcb0b4d7b8c72214cb7b971d884510e8bd91",
                                "image": "mongo:latest",
                                "imageID": "docker-pullable://mongo@sha256:f025ed224f93086ce4ddc8f61a4aa8113e8dcd6106ca0e3a599f9a0d76ab94ad",
                                "lastState": {},
                                "name": "orders-db",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:40:54Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.133",
                        "phase": "Running",
                        "podIP": "172.20.2.4",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:50Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:50Z",
                        "generateName": "payment-7779bc549c-",
                        "labels": {
                            "name": "payment",
                            "pod-template-hash": "7779bc549c"
                        },
                        "name": "payment-7779bc549c-bbf2l",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "payment-7779bc549c",
                                "uid": "1aa73282-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "1735",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/payment-7779bc549c-bbf2l",
                        "uid": "1aa7e498-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "image": "weaveworksdemos/payment:0.4.3",
                                "imagePullPolicy": "IfNotPresent",
                                "name": "payment",
                                "ports": [
                                    {
                                        "containerPort": 80,
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "securityContext": {
                                    "capabilities": {
                                        "add": [
                                            "NET_BIND_SERVICE"
                                        ],
                                        "drop": [
                                            "all"
                                        ]
                                    },
                                    "procMount": "Default",
                                    "readOnlyRootFilesystem": true,
                                    "runAsNonRoot": true,
                                    "runAsUser": 10001
                                },
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.205",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:50Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:39:10Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:39:10Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:50Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://d0389e93b6e73065ed55b7561790610dbb0467d26597e2ca3a9aedb6d0996e59",
                                "image": "weaveworksdemos/payment:0.4.3",
                                "imageID": "docker-pullable://weaveworksdemos/payment@sha256:5ab1c9877480a018d4dda10d6dfa382776e6bca9fc1c60bacbb80903fde8cfe0",
                                "lastState": {},
                                "name": "payment",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:39:10Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.205",
                        "phase": "Running",
                        "podIP": "172.20.1.5",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:50Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:50Z",
                        "generateName": "queue-master-6bb75d8867-",
                        "labels": {
                            "name": "queue-master",
                            "pod-template-hash": "6bb75d8867"
                        },
                        "name": "queue-master-6bb75d8867-8h5w9",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "queue-master-6bb75d8867",
                                "uid": "1ae46b85-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "2226",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/queue-master-6bb75d8867-8h5w9",
                        "uid": "1ae73eab-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "image": "weaveworksdemos/queue-master:0.3.1",
                                "imagePullPolicy": "IfNotPresent",
                                "name": "queue-master",
                                "ports": [
                                    {
                                        "containerPort": 80,
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.133",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:51Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:43:51Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:43:51Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:50Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://638106b5fba50332e6c3ce83c9774798772057cc1fe24955b7090fe3c6abd8d8",
                                "image": "weaveworksdemos/queue-master:0.3.1",
                                "imageID": "docker-pullable://weaveworksdemos/queue-master@sha256:6292d3095f4c7aeed8d863527f8ef6d7a75d3128f20fc61e57f398c100142712",
                                "lastState": {},
                                "name": "queue-master",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:43:51Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.133",
                        "phase": "Running",
                        "podIP": "172.20.2.5",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:51Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:51Z",
                        "generateName": "rabbitmq-549bb9596f-",
                        "labels": {
                            "name": "rabbitmq",
                            "pod-template-hash": "549bb9596f"
                        },
                        "name": "rabbitmq-549bb9596f-znnfn",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "rabbitmq-549bb9596f",
                                "uid": "1b281cf4-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "1682",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/rabbitmq-549bb9596f-znnfn",
                        "uid": "1b298bdc-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "image": "rabbitmq:3.6.8",
                                "imagePullPolicy": "IfNotPresent",
                                "name": "rabbitmq",
                                "ports": [
                                    {
                                        "containerPort": 5672,
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "securityContext": {
                                    "capabilities": {
                                        "add": [
                                            "CHOWN",
                                            "SETGID",
                                            "SETUID",
                                            "DAC_OVERRIDE"
                                        ],
                                        "drop": [
                                            "all"
                                        ]
                                    },
                                    "procMount": "Default",
                                    "readOnlyRootFilesystem": true
                                },
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.206",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:51Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:38:42Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:38:42Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:51Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://c3eaafa89c26ae010f368693f1151cc27626ec204f5df780cffc6b016c959c69",
                                "image": "rabbitmq:3.6.8",
                                "imageID": "docker-pullable://rabbitmq@sha256:a9f4923559bbcd00b93b02e61615aef5eb6f1d1c98db51053bab0fa6b680db26",
                                "lastState": {},
                                "name": "rabbitmq",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:38:41Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.206",
                        "phase": "Running",
                        "podIP": "172.20.3.5",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:51Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:51Z",
                        "generateName": "shipping-65769d99d7-",
                        "labels": {
                            "name": "shipping",
                            "pod-template-hash": "65769d99d7"
                        },
                        "name": "shipping-65769d99d7-stxwm",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "shipping-65769d99d7",
                                "uid": "1b711738-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "1908",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/shipping-65769d99d7-stxwm",
                        "uid": "1b73afef-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "env": [
                                    {
                                        "name": "ZIPKIN",
                                        "value": "zipkin.jaeger.svc.cluster.local"
                                    },
                                    {
                                        "name": "JAVA_OPTS",
                                        "value": "-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom"
                                    }
                                ],
                                "image": "weaveworksdemos/shipping:0.4.8",
                                "imagePullPolicy": "IfNotPresent",
                                "name": "shipping",
                                "ports": [
                                    {
                                        "containerPort": 80,
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "securityContext": {
                                    "capabilities": {
                                        "add": [
                                            "NET_BIND_SERVICE"
                                        ],
                                        "drop": [
                                            "all"
                                        ]
                                    },
                                    "procMount": "Default",
                                    "readOnlyRootFilesystem": true,
                                    "runAsNonRoot": true,
                                    "runAsUser": 10001
                                },
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/tmp",
                                        "name": "tmp-volume"
                                    },
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.188",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "emptyDir": {
                                    "medium": "Memory"
                                },
                                "name": "tmp-volume"
                            },
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:52Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:40:43Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:40:43Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:51Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://9553294fea306a80a2b7c0c6cf613f6f51c1fd7d119366052485f2c885aba98a",
                                "image": "weaveworksdemos/shipping:0.4.8",
                                "imageID": "docker-pullable://weaveworksdemos/shipping@sha256:983305c948fded487f4a4acdeab5f898e89d577b4bc1ca3de7750076469ccad4",
                                "lastState": {},
                                "name": "shipping",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:40:42Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.188",
                        "phase": "Running",
                        "podIP": "172.20.4.5",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:52Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:52Z",
                        "generateName": "user-6b445f9b5b-",
                        "labels": {
                            "name": "user",
                            "pod-template-hash": "6b445f9b5b"
                        },
                        "name": "user-6b445f9b5b-65rzk",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "user-6b445f9b5b",
                                "uid": "1bf8db2c-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "2371",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/user-6b445f9b5b-65rzk",
                        "uid": "1bfe2dc5-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "env": [
                                    {
                                        "name": "MONGO_HOST",
                                        "value": "user-db:27017"
                                    }
                                ],
                                "image": "weaveworksdemos/user:0.4.7",
                                "imagePullPolicy": "IfNotPresent",
                                "name": "user",
                                "ports": [
                                    {
                                        "containerPort": 80,
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "securityContext": {
                                    "capabilities": {
                                        "add": [
                                            "NET_BIND_SERVICE"
                                        ],
                                        "drop": [
                                            "all"
                                        ]
                                    },
                                    "procMount": "Default",
                                    "readOnlyRootFilesystem": true,
                                    "runAsNonRoot": true,
                                    "runAsUser": 10001
                                },
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.133",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:52Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:45:16Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:45:16Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:52Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://8e9acd437943f631d0e7a0c052c72897cf95ffd579bd17e8f0c05cb51014c207",
                                "image": "weaveworksdemos/user:0.4.7",
                                "imageID": "docker-pullable://weaveworksdemos/user@sha256:2ffccc332963c89e035fea52201012208bf62df43a55fe461ad6598a5c757ab7",
                                "lastState": {},
                                "name": "user",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:45:15Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.133",
                        "phase": "Running",
                        "podIP": "172.20.2.6",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:52Z"
                    }
                },
                {
                    "metadata": {
                        "creationTimestamp": "2019-04-03T07:35:52Z",
                        "generateName": "user-db-56bbb4c6db-",
                        "labels": {
                            "name": "user-db",
                            "pod-template-hash": "56bbb4c6db"
                        },
                        "name": "user-db-56bbb4c6db-lx4v8",
                        "namespace": "sock-shop",
                        "ownerReferences": [
                            {
                                "apiVersion": "apps/v1",
                                "blockOwnerDeletion": true,
                                "controller": true,
                                "kind": "ReplicaSet",
                                "name": "user-db-56bbb4c6db",
                                "uid": "1bb0827f-55e3-11e9-a74e-002481eeda4c"
                            }
                        ],
                        "resourceVersion": "2058",
                        "selfLink": "/api/v1/namespaces/sock-shop/pods/user-db-56bbb4c6db-lx4v8",
                        "uid": "1bb5c530-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "containers": [
                            {
                                "image": "weaveworksdemos/user-db:0.4.0",
                                "imagePullPolicy": "IfNotPresent",
                                "name": "user-db",
                                "ports": [
                                    {
                                        "containerPort": 27017,
                                        "name": "mongo",
                                        "protocol": "TCP"
                                    }
                                ],
                                "resources": {},
                                "securityContext": {
                                    "capabilities": {
                                        "add": [
                                            "CHOWN",
                                            "SETGID",
                                            "SETUID"
                                        ],
                                        "drop": [
                                            "all"
                                        ]
                                    },
                                    "procMount": "Default",
                                    "readOnlyRootFilesystem": true
                                },
                                "terminationMessagePath": "/dev/termination-log",
                                "terminationMessagePolicy": "File",
                                "volumeMounts": [
                                    {
                                        "mountPath": "/tmp",
                                        "name": "tmp-volume"
                                    },
                                    {
                                        "mountPath": "/var/run/secrets/kubernetes.io/serviceaccount",
                                        "name": "default-token-vmkdl",
                                        "readOnly": true
                                    }
                                ]
                            }
                        ],
                        "dnsPolicy": "ClusterFirst",
                        "enableServiceLinks": true,
                        "nodeName": "192.168.199.205",
                        "nodeSelector": {
                            "beta.kubernetes.io/os": "linux"
                        },
                        "restartPolicy": "Always",
                        "schedulerName": "default-scheduler",
                        "securityContext": {},
                        "serviceAccount": "default",
                        "serviceAccountName": "default",
                        "terminationGracePeriodSeconds": 30,
                        "volumes": [
                            {
                                "emptyDir": {
                                    "medium": "Memory"
                                },
                                "name": "tmp-volume"
                            },
                            {
                                "name": "default-token-vmkdl",
                                "secret": {
                                    "defaultMode": 420,
                                    "secretName": "default-token-vmkdl"
                                }
                            }
                        ]
                    },
                    "status": {
                        "conditions": [
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:52Z",
                                "status": "True",
                                "type": "Initialized"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:42:11Z",
                                "status": "True",
                                "type": "Ready"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:42:11Z",
                                "status": "True",
                                "type": "ContainersReady"
                            },
                            {
                                "lastProbeTime": null,
                                "lastTransitionTime": "2019-04-03T07:35:52Z",
                                "status": "True",
                                "type": "PodScheduled"
                            }
                        ],
                        "containerStatuses": [
                            {
                                "containerID": "docker://db74be5ec15f26743862cf32589584dee8c9633eccf32b64db7b3710e8f8eb17",
                                "image": "weaveworksdemos/user-db:0.4.0",
                                "imageID": "docker-pullable://weaveworksdemos/user-db@sha256:b43f0f8a76e0c908805fcec74d1ad7f4af4d93c4612632bd6dc20a87508e0b68",
                                "lastState": {},
                                "name": "user-db",
                                "ready": true,
                                "restartCount": 0,
                                "state": {
                                    "running": {
                                        "startedAt": "2019-04-03T07:42:10Z"
                                    }
                                }
                            }
                        ],
                        "hostIP": "192.168.199.205",
                        "phase": "Running",
                        "podIP": "172.20.1.6",
                        "qosClass": "BestEffort",
                        "startTime": "2019-04-03T07:35:52Z"
                    }
                }
            ]
        }
    },
    "failed": {},
    "skipped": {},
    "status": {},
    "success": [
        {
            "creationTimestamp": "2019-04-03T07:35:48Z",
            "hostIP": "192.168.199.206",
            "labels": {
                "name": "carts",
                "pod-template-hash": "648d5f498d"
            },
            "name": "carts-648d5f498d-tgq2k",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.206",
            "podIP": "172.20.3.4"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:47Z",
            "hostIP": "192.168.199.133",
            "labels": {
                "name": "carts-db",
                "pod-template-hash": "64b6cc584f"
            },
            "name": "carts-db-64b6cc584f-6tbvj",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.133",
            "podIP": "172.20.2.2"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:49Z",
            "hostIP": "192.168.199.188",
            "labels": {
                "name": "catalogue",
                "pod-template-hash": "6759fc9bf5"
            },
            "name": "catalogue-6759fc9bf5-9nfjb",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.188",
            "podIP": "172.20.4.3"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:48Z",
            "hostIP": "192.168.199.133",
            "labels": {
                "name": "catalogue-db",
                "pod-template-hash": "99cbcbb88"
            },
            "name": "catalogue-db-99cbcbb88-8wdp5",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.133",
            "podIP": "172.20.2.3"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:49Z",
            "hostIP": "192.168.199.205",
            "labels": {
                "name": "front-end",
                "pod-template-hash": "77b48955b6"
            },
            "name": "front-end-77b48955b6-spjsh",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.205",
            "podIP": "172.20.1.4"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:50Z",
            "hostIP": "192.168.199.188",
            "labels": {
                "name": "orders",
                "pod-template-hash": "6496fcd6f7"
            },
            "name": "orders-6496fcd6f7-rz24g",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.188",
            "podIP": "172.20.4.4"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:49Z",
            "hostIP": "192.168.199.133",
            "labels": {
                "name": "orders-db",
                "pod-template-hash": "86f5c494b9"
            },
            "name": "orders-db-86f5c494b9-v8fkr",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.133",
            "podIP": "172.20.2.4"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:50Z",
            "hostIP": "192.168.199.205",
            "labels": {
                "name": "payment",
                "pod-template-hash": "7779bc549c"
            },
            "name": "payment-7779bc549c-bbf2l",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.205",
            "podIP": "172.20.1.5"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:50Z",
            "hostIP": "192.168.199.133",
            "labels": {
                "name": "queue-master",
                "pod-template-hash": "6bb75d8867"
            },
            "name": "queue-master-6bb75d8867-8h5w9",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.133",
            "podIP": "172.20.2.5"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:51Z",
            "hostIP": "192.168.199.206",
            "labels": {
                "name": "rabbitmq",
                "pod-template-hash": "549bb9596f"
            },
            "name": "rabbitmq-549bb9596f-znnfn",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.206",
            "podIP": "172.20.3.5"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:51Z",
            "hostIP": "192.168.199.188",
            "labels": {
                "name": "shipping",
                "pod-template-hash": "65769d99d7"
            },
            "name": "shipping-65769d99d7-stxwm",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.188",
            "podIP": "172.20.4.5"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:52Z",
            "hostIP": "192.168.199.133",
            "labels": {
                "name": "user",
                "pod-template-hash": "6b445f9b5b"
            },
            "name": "user-6b445f9b5b-65rzk",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.133",
            "podIP": "172.20.2.6"
        },
        {
            "creationTimestamp": "2019-04-03T07:35:52Z",
            "hostIP": "192.168.199.205",
            "labels": {
                "name": "user-db",
                "pod-template-hash": "56bbb4c6db"
            },
            "name": "user-db-56bbb4c6db-lx4v8",
            "namespace": "sock-shop",
            "nodeName": "192.168.199.205",
            "podIP": "172.20.1.6"
        }
    ],
    "unreachable": {}
}
```

#### tool/api/v1.0/get_svc/sock-shop

```json
{
    "detail": {
        "10.60.38.181": {
            "_ansible_no_log": false,
            "_ansible_parsed": true,
            "changed": false,
            "invocation": {
                "module_args": {
                    "api_key": null,
                    "api_version": "v1",
                    "cert_file": null,
                    "context": null,
                    "field_selectors": [],
                    "host": null,
                    "key_file": null,
                    "kind": "Service",
                    "kubeconfig": null,
                    "label_selectors": [],
                    "name": null,
                    "namespace": "sock-shop",
                    "password": null,
                    "ssl_ca_cert": null,
                    "username": null,
                    "verify_ssl": null
                }
            },
            "resources": [
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"carts\"},\"name\":\"carts\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":80,\"targetPort\":80}],\"selector\":{\"name\":\"carts\"}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:48Z",
                        "labels": {
                            "name": "carts"
                        },
                        "name": "carts",
                        "namespace": "sock-shop",
                        "resourceVersion": "1181",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/carts",
                        "uid": "1961e804-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.91.177",
                        "ports": [
                            {
                                "port": 80,
                                "protocol": "TCP",
                                "targetPort": 80
                            }
                        ],
                        "selector": {
                            "name": "carts"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"carts-db\"},\"name\":\"carts-db\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":27017,\"targetPort\":27017}],\"selector\":{\"name\":\"carts-db\"}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:47Z",
                        "labels": {
                            "name": "carts-db"
                        },
                        "name": "carts-db",
                        "namespace": "sock-shop",
                        "resourceVersion": "1165",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/carts-db",
                        "uid": "191dfe88-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.178.205",
                        "ports": [
                            {
                                "port": 27017,
                                "protocol": "TCP",
                                "targetPort": 27017
                            }
                        ],
                        "selector": {
                            "name": "carts-db"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"catalogue\"},\"name\":\"catalogue\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":80,\"targetPort\":80}],\"selector\":{\"name\":\"catalogue\"}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:49Z",
                        "labels": {
                            "name": "catalogue"
                        },
                        "name": "catalogue",
                        "namespace": "sock-shop",
                        "resourceVersion": "1211",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/catalogue",
                        "uid": "19d1e6ca-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.106.21",
                        "ports": [
                            {
                                "port": 80,
                                "protocol": "TCP",
                                "targetPort": 80
                            }
                        ],
                        "selector": {
                            "name": "catalogue"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"catalogue-db\"},\"name\":\"catalogue-db\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":3306,\"targetPort\":3306}],\"selector\":{\"name\":\"catalogue-db\"}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:48Z",
                        "labels": {
                            "name": "catalogue-db"
                        },
                        "name": "catalogue-db",
                        "namespace": "sock-shop",
                        "resourceVersion": "1197",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/catalogue-db",
                        "uid": "19aad493-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.5.119",
                        "ports": [
                            {
                                "port": 3306,
                                "protocol": "TCP",
                                "targetPort": 3306
                            }
                        ],
                        "selector": {
                            "name": "catalogue-db"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"front-end\"},\"name\":\"front-end\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"nodePort\":30001,\"port\":80,\"targetPort\":8079}],\"selector\":{\"name\":\"front-end\"},\"type\":\"NodePort\"}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:49Z",
                        "labels": {
                            "name": "front-end"
                        },
                        "name": "front-end",
                        "namespace": "sock-shop",
                        "resourceVersion": "1231",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/front-end",
                        "uid": "1a1fc33e-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.52.112",
                        "externalTrafficPolicy": "Cluster",
                        "ports": [
                            {
                                "nodePort": 30001,
                                "port": 80,
                                "protocol": "TCP",
                                "targetPort": 8079
                            }
                        ],
                        "selector": {
                            "name": "front-end"
                        },
                        "sessionAffinity": "None",
                        "type": "NodePort"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"orders\"},\"name\":\"orders\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":80,\"targetPort\":80}],\"selector\":{\"name\":\"orders\"}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:50Z",
                        "labels": {
                            "name": "orders"
                        },
                        "name": "orders",
                        "namespace": "sock-shop",
                        "resourceVersion": "1262",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/orders",
                        "uid": "1a86dfc6-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.102.240",
                        "ports": [
                            {
                                "port": 80,
                                "protocol": "TCP",
                                "targetPort": 80
                            }
                        ],
                        "selector": {
                            "name": "orders"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"orders-db\"},\"name\":\"orders-db\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":27017,\"targetPort\":27017}],\"selector\":{\"name\":\"orders-db\"}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:49Z",
                        "labels": {
                            "name": "orders-db"
                        },
                        "name": "orders-db",
                        "namespace": "sock-shop",
                        "resourceVersion": "1245",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/orders-db",
                        "uid": "1a55179e-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.3.223",
                        "ports": [
                            {
                                "port": 27017,
                                "protocol": "TCP",
                                "targetPort": 27017
                            }
                        ],
                        "selector": {
                            "name": "orders-db"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"payment\"},\"name\":\"payment\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":80,\"targetPort\":80}],\"selector\":{\"name\":\"payment\"}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:50Z",
                        "labels": {
                            "name": "payment"
                        },
                        "name": "payment",
                        "namespace": "sock-shop",
                        "resourceVersion": "1281",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/payment",
                        "uid": "1ada71e4-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.246.201",
                        "ports": [
                            {
                                "port": 80,
                                "protocol": "TCP",
                                "targetPort": 80
                            }
                        ],
                        "selector": {
                            "name": "payment"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{\"prometheus.io/path\":\"/prometheus\"},\"labels\":{\"name\":\"queue-master\"},\"name\":\"queue-master\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":80,\"targetPort\":80}],\"selector\":{\"name\":\"queue-master\"}}}\n",
                            "prometheus.io/path": "/prometheus"
                        },
                        "creationTimestamp": "2019-04-03T07:35:51Z",
                        "labels": {
                            "name": "queue-master"
                        },
                        "name": "queue-master",
                        "namespace": "sock-shop",
                        "resourceVersion": "1296",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/queue-master",
                        "uid": "1b084c4e-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.168.90",
                        "ports": [
                            {
                                "port": 80,
                                "protocol": "TCP",
                                "targetPort": 80
                            }
                        ],
                        "selector": {
                            "name": "queue-master"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"rabbitmq\"},\"name\":\"rabbitmq\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":5672,\"targetPort\":5672}],\"selector\":{\"name\":\"rabbitmq\"}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:51Z",
                        "labels": {
                            "name": "rabbitmq"
                        },
                        "name": "rabbitmq",
                        "namespace": "sock-shop",
                        "resourceVersion": "1310",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/rabbitmq",
                        "uid": "1b4e330f-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.2.56",
                        "ports": [
                            {
                                "port": 5672,
                                "protocol": "TCP",
                                "targetPort": 5672
                            }
                        ],
                        "selector": {
                            "name": "rabbitmq"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"shipping\"},\"name\":\"shipping\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":80,\"targetPort\":80}],\"selector\":{\"name\":\"shipping\"}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:51Z",
                        "labels": {
                            "name": "shipping"
                        },
                        "name": "shipping",
                        "namespace": "sock-shop",
                        "resourceVersion": "1328",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/shipping",
                        "uid": "1b8bdba1-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.93.138",
                        "ports": [
                            {
                                "port": 80,
                                "protocol": "TCP",
                                "targetPort": 80
                            }
                        ],
                        "selector": {
                            "name": "shipping"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"user\"},\"name\":\"user\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":80,\"targetPort\":80}],\"selector\":{\"name\":\"user\"}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:52Z",
                        "labels": {
                            "name": "user"
                        },
                        "name": "user",
                        "namespace": "sock-shop",
                        "resourceVersion": "1371",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/user",
                        "uid": "1c19fbb0-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.14.126",
                        "ports": [
                            {
                                "port": 80,
                                "protocol": "TCP",
                                "targetPort": 80
                            }
                        ],
                        "selector": {
                            "name": "user"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"v1\",\"kind\":\"Service\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"user-db\"},\"name\":\"user-db\",\"namespace\":\"sock-shop\"},\"spec\":{\"ports\":[{\"port\":27017,\"targetPort\":27017}],\"selector\":{\"name\":\"user-db\"}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:52Z",
                        "labels": {
                            "name": "user-db"
                        },
                        "name": "user-db",
                        "namespace": "sock-shop",
                        "resourceVersion": "1351",
                        "selfLink": "/api/v1/namespaces/sock-shop/services/user-db",
                        "uid": "1bd63826-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "clusterIP": "10.68.68.66",
                        "ports": [
                            {
                                "port": 27017,
                                "protocol": "TCP",
                                "targetPort": 27017
                            }
                        ],
                        "selector": {
                            "name": "user-db"
                        },
                        "sessionAffinity": "None",
                        "type": "ClusterIP"
                    },
                    "status": {
                        "loadBalancer": {}
                    }
                }
            ]
        }
    },
    "failed": {},
    "skipped": {},
    "status": {},
    "success": [
        {
            "clusterIP": "10.68.91.177",
            "creationTimestamp": "2019-04-03T07:35:48Z",
            "labels": {
                "name": "carts"
            },
            "name": "carts",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.178.205",
            "creationTimestamp": "2019-04-03T07:35:47Z",
            "labels": {
                "name": "carts-db"
            },
            "name": "carts-db",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.106.21",
            "creationTimestamp": "2019-04-03T07:35:49Z",
            "labels": {
                "name": "catalogue"
            },
            "name": "catalogue",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.5.119",
            "creationTimestamp": "2019-04-03T07:35:48Z",
            "labels": {
                "name": "catalogue-db"
            },
            "name": "catalogue-db",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.52.112",
            "creationTimestamp": "2019-04-03T07:35:49Z",
            "labels": {
                "name": "front-end"
            },
            "name": "front-end",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.102.240",
            "creationTimestamp": "2019-04-03T07:35:50Z",
            "labels": {
                "name": "orders"
            },
            "name": "orders",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.3.223",
            "creationTimestamp": "2019-04-03T07:35:49Z",
            "labels": {
                "name": "orders-db"
            },
            "name": "orders-db",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.246.201",
            "creationTimestamp": "2019-04-03T07:35:50Z",
            "labels": {
                "name": "payment"
            },
            "name": "payment",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.168.90",
            "creationTimestamp": "2019-04-03T07:35:51Z",
            "labels": {
                "name": "queue-master"
            },
            "name": "queue-master",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.2.56",
            "creationTimestamp": "2019-04-03T07:35:51Z",
            "labels": {
                "name": "rabbitmq"
            },
            "name": "rabbitmq",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.93.138",
            "creationTimestamp": "2019-04-03T07:35:51Z",
            "labels": {
                "name": "shipping"
            },
            "name": "shipping",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.14.126",
            "creationTimestamp": "2019-04-03T07:35:52Z",
            "labels": {
                "name": "user"
            },
            "name": "user",
            "namespace": "sock-shop"
        },
        {
            "clusterIP": "10.68.68.66",
            "creationTimestamp": "2019-04-03T07:35:52Z",
            "labels": {
                "name": "user-db"
            },
            "name": "user-db",
            "namespace": "sock-shop"
        }
    ],
    "unreachable": {}
}
```

#### tool/api/v1.0/get_deployment/sock-shop

```json
{
    "detail": {
        "10.60.38.181": {
            "_ansible_no_log": false,
            "_ansible_parsed": true,
            "changed": false,
            "invocation": {
                "module_args": {
                    "api_key": null,
                    "api_version": "v1",
                    "cert_file": null,
                    "context": null,
                    "field_selectors": [],
                    "host": null,
                    "key_file": null,
                    "kind": "Deployment",
                    "kubeconfig": null,
                    "label_selectors": [],
                    "name": null,
                    "namespace": "sock-shop",
                    "password": null,
                    "ssl_ca_cert": null,
                    "username": null,
                    "verify_ssl": null
                }
            },
            "resources": [
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"carts\"},\"name\":\"carts\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"carts\"}},\"spec\":{\"containers\":[{\"env\":[{\"name\":\"ZIPKIN\",\"value\":\"zipkin.jaeger.svc.cluster.local\"},{\"name\":\"JAVA_OPTS\",\"value\":\"-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom\"}],\"image\":\"weaveworksdemos/carts:0.4.8\",\"name\":\"carts\",\"ports\":[{\"containerPort\":80}],\"securityContext\":{\"capabilities\":{\"add\":[\"NET_BIND_SERVICE\"],\"drop\":[\"all\"]},\"readOnlyRootFilesystem\":true,\"runAsNonRoot\":true,\"runAsUser\":10001},\"volumeMounts\":[{\"mountPath\":\"/tmp\",\"name\":\"tmp-volume\"}]}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"},\"volumes\":[{\"emptyDir\":{\"medium\":\"Memory\"},\"name\":\"tmp-volume\"}]}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:48Z",
                        "generation": 1,
                        "labels": {
                            "name": "carts"
                        },
                        "name": "carts",
                        "namespace": "sock-shop",
                        "resourceVersion": "1489",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/carts",
                        "uid": "19358f6b-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "carts"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "carts"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "env": [
                                            {
                                                "name": "ZIPKIN",
                                                "value": "zipkin.jaeger.svc.cluster.local"
                                            },
                                            {
                                                "name": "JAVA_OPTS",
                                                "value": "-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom"
                                            }
                                        ],
                                        "image": "weaveworksdemos/carts:0.4.8",
                                        "imagePullPolicy": "IfNotPresent",
                                        "name": "carts",
                                        "ports": [
                                            {
                                                "containerPort": 80,
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "securityContext": {
                                            "capabilities": {
                                                "add": [
                                                    "NET_BIND_SERVICE"
                                                ],
                                                "drop": [
                                                    "all"
                                                ]
                                            },
                                            "procMount": "Default",
                                            "readOnlyRootFilesystem": true,
                                            "runAsNonRoot": true,
                                            "runAsUser": 10001
                                        },
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File",
                                        "volumeMounts": [
                                            {
                                                "mountPath": "/tmp",
                                                "name": "tmp-volume"
                                            }
                                        ]
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30,
                                "volumes": [
                                    {
                                        "emptyDir": {
                                            "medium": "Memory"
                                        },
                                        "name": "tmp-volume"
                                    }
                                ]
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:48Z",
                                "lastUpdateTime": "2019-04-03T07:35:48Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"carts-db\"},\"name\":\"carts-db\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"carts-db\"}},\"spec\":{\"containers\":[{\"image\":\"mongo\",\"name\":\"carts-db\",\"ports\":[{\"containerPort\":27017,\"name\":\"mongo\"}],\"securityContext\":{\"capabilities\":{\"add\":[\"CHOWN\",\"SETGID\",\"SETUID\"],\"drop\":[\"all\"]},\"readOnlyRootFilesystem\":true},\"volumeMounts\":[{\"mountPath\":\"/tmp\",\"name\":\"tmp-volume\"}]}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"},\"volumes\":[{\"emptyDir\":{\"medium\":\"Memory\"},\"name\":\"tmp-volume\"}]}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:47Z",
                        "generation": 1,
                        "labels": {
                            "name": "carts-db"
                        },
                        "name": "carts-db",
                        "namespace": "sock-shop",
                        "resourceVersion": "1627",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/carts-db",
                        "uid": "190050e8-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "carts-db"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "carts-db"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "image": "mongo",
                                        "imagePullPolicy": "Always",
                                        "name": "carts-db",
                                        "ports": [
                                            {
                                                "containerPort": 27017,
                                                "name": "mongo",
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "securityContext": {
                                            "capabilities": {
                                                "add": [
                                                    "CHOWN",
                                                    "SETGID",
                                                    "SETUID"
                                                ],
                                                "drop": [
                                                    "all"
                                                ]
                                            },
                                            "procMount": "Default",
                                            "readOnlyRootFilesystem": true
                                        },
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File",
                                        "volumeMounts": [
                                            {
                                                "mountPath": "/tmp",
                                                "name": "tmp-volume"
                                            }
                                        ]
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30,
                                "volumes": [
                                    {
                                        "emptyDir": {
                                            "medium": "Memory"
                                        },
                                        "name": "tmp-volume"
                                    }
                                ]
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:47Z",
                                "lastUpdateTime": "2019-04-03T07:35:47Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"catalogue\"},\"name\":\"catalogue\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"catalogue\"}},\"spec\":{\"containers\":[{\"image\":\"weaveworksdemos/catalogue:0.3.5\",\"name\":\"catalogue\",\"ports\":[{\"containerPort\":80}],\"securityContext\":{\"capabilities\":{\"add\":[\"NET_BIND_SERVICE\"],\"drop\":[\"all\"]},\"readOnlyRootFilesystem\":true,\"runAsNonRoot\":true,\"runAsUser\":10001}}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"}}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:48Z",
                        "generation": 1,
                        "labels": {
                            "name": "catalogue"
                        },
                        "name": "catalogue",
                        "namespace": "sock-shop",
                        "resourceVersion": "1549",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/catalogue",
                        "uid": "19c348f9-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "catalogue"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "catalogue"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "image": "weaveworksdemos/catalogue:0.3.5",
                                        "imagePullPolicy": "IfNotPresent",
                                        "name": "catalogue",
                                        "ports": [
                                            {
                                                "containerPort": 80,
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "securityContext": {
                                            "capabilities": {
                                                "add": [
                                                    "NET_BIND_SERVICE"
                                                ],
                                                "drop": [
                                                    "all"
                                                ]
                                            },
                                            "procMount": "Default",
                                            "readOnlyRootFilesystem": true,
                                            "runAsNonRoot": true,
                                            "runAsUser": 10001
                                        },
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File"
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:49Z",
                                "lastUpdateTime": "2019-04-03T07:35:49Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"catalogue-db\"},\"name\":\"catalogue-db\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"catalogue-db\"}},\"spec\":{\"containers\":[{\"env\":[{\"name\":\"MYSQL_ROOT_PASSWORD\",\"value\":\"fake_password\"},{\"name\":\"MYSQL_DATABASE\",\"value\":\"socksdb\"}],\"image\":\"weaveworksdemos/catalogue-db:0.3.0\",\"name\":\"catalogue-db\",\"ports\":[{\"containerPort\":3306,\"name\":\"mysql\"}]}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"}}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:48Z",
                        "generation": 1,
                        "labels": {
                            "name": "catalogue-db"
                        },
                        "name": "catalogue-db",
                        "namespace": "sock-shop",
                        "resourceVersion": "1840",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/catalogue-db",
                        "uid": "1983e492-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "catalogue-db"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "catalogue-db"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "env": [
                                            {
                                                "name": "MYSQL_ROOT_PASSWORD",
                                                "value": "fake_password"
                                            },
                                            {
                                                "name": "MYSQL_DATABASE",
                                                "value": "socksdb"
                                            }
                                        ],
                                        "image": "weaveworksdemos/catalogue-db:0.3.0",
                                        "imagePullPolicy": "IfNotPresent",
                                        "name": "catalogue-db",
                                        "ports": [
                                            {
                                                "containerPort": 3306,
                                                "name": "mysql",
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File"
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:48Z",
                                "lastUpdateTime": "2019-04-03T07:35:48Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"name\":\"front-end\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"front-end\"}},\"spec\":{\"containers\":[{\"image\":\"weaveworksdemos/front-end:0.3.12\",\"name\":\"front-end\",\"ports\":[{\"containerPort\":8079}],\"resources\":{\"requests\":{\"cpu\":\"100m\",\"memory\":\"100Mi\"}},\"securityContext\":{\"capabilities\":{\"drop\":[\"all\"]},\"readOnlyRootFilesystem\":true,\"runAsNonRoot\":true,\"runAsUser\":10001}}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"}}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:49Z",
                        "generation": 1,
                        "labels": {
                            "name": "front-end"
                        },
                        "name": "front-end",
                        "namespace": "sock-shop",
                        "resourceVersion": "1580",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/front-end",
                        "uid": "19ef1308-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "front-end"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "front-end"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "image": "weaveworksdemos/front-end:0.3.12",
                                        "imagePullPolicy": "IfNotPresent",
                                        "name": "front-end",
                                        "ports": [
                                            {
                                                "containerPort": 8079,
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {
                                            "requests": {
                                                "cpu": "100m",
                                                "memory": "100Mi"
                                            }
                                        },
                                        "securityContext": {
                                            "capabilities": {
                                                "drop": [
                                                    "all"
                                                ]
                                            },
                                            "procMount": "Default",
                                            "readOnlyRootFilesystem": true,
                                            "runAsNonRoot": true,
                                            "runAsUser": 10001
                                        },
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File"
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:49Z",
                                "lastUpdateTime": "2019-04-03T07:35:49Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"orders\"},\"name\":\"orders\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"orders\"}},\"spec\":{\"containers\":[{\"env\":[{\"name\":\"ZIPKIN\",\"value\":\"zipkin.jaeger.svc.cluster.local\"},{\"name\":\"JAVA_OPTS\",\"value\":\"-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom\"}],\"image\":\"weaveworksdemos/orders:0.4.7\",\"name\":\"orders\",\"ports\":[{\"containerPort\":80}],\"securityContext\":{\"capabilities\":{\"add\":[\"NET_BIND_SERVICE\"],\"drop\":[\"all\"]},\"readOnlyRootFilesystem\":true,\"runAsNonRoot\":true,\"runAsUser\":10001},\"volumeMounts\":[{\"mountPath\":\"/tmp\",\"name\":\"tmp-volume\"}]}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"},\"volumes\":[{\"emptyDir\":{\"medium\":\"Memory\"},\"name\":\"tmp-volume\"}]}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:49Z",
                        "generation": 1,
                        "labels": {
                            "name": "orders"
                        },
                        "name": "orders",
                        "namespace": "sock-shop",
                        "resourceVersion": "1759",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/orders",
                        "uid": "1a5d7854-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "orders"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "orders"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "env": [
                                            {
                                                "name": "ZIPKIN",
                                                "value": "zipkin.jaeger.svc.cluster.local"
                                            },
                                            {
                                                "name": "JAVA_OPTS",
                                                "value": "-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom"
                                            }
                                        ],
                                        "image": "weaveworksdemos/orders:0.4.7",
                                        "imagePullPolicy": "IfNotPresent",
                                        "name": "orders",
                                        "ports": [
                                            {
                                                "containerPort": 80,
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "securityContext": {
                                            "capabilities": {
                                                "add": [
                                                    "NET_BIND_SERVICE"
                                                ],
                                                "drop": [
                                                    "all"
                                                ]
                                            },
                                            "procMount": "Default",
                                            "readOnlyRootFilesystem": true,
                                            "runAsNonRoot": true,
                                            "runAsUser": 10001
                                        },
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File",
                                        "volumeMounts": [
                                            {
                                                "mountPath": "/tmp",
                                                "name": "tmp-volume"
                                            }
                                        ]
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30,
                                "volumes": [
                                    {
                                        "emptyDir": {
                                            "medium": "Memory"
                                        },
                                        "name": "tmp-volume"
                                    }
                                ]
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:50Z",
                                "lastUpdateTime": "2019-04-03T07:35:50Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"orders-db\"},\"name\":\"orders-db\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"orders-db\"}},\"spec\":{\"containers\":[{\"image\":\"mongo\",\"name\":\"orders-db\",\"ports\":[{\"containerPort\":27017,\"name\":\"mongo\"}],\"securityContext\":{\"capabilities\":{\"add\":[\"CHOWN\",\"SETGID\",\"SETUID\"],\"drop\":[\"all\"]},\"readOnlyRootFilesystem\":true},\"volumeMounts\":[{\"mountPath\":\"/tmp\",\"name\":\"tmp-volume\"}]}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"},\"volumes\":[{\"emptyDir\":{\"medium\":\"Memory\"},\"name\":\"tmp-volume\"}]}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:49Z",
                        "generation": 1,
                        "labels": {
                            "name": "orders-db"
                        },
                        "name": "orders-db",
                        "namespace": "sock-shop",
                        "resourceVersion": "1936",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/orders-db",
                        "uid": "1a392dfb-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "orders-db"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "orders-db"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "image": "mongo",
                                        "imagePullPolicy": "Always",
                                        "name": "orders-db",
                                        "ports": [
                                            {
                                                "containerPort": 27017,
                                                "name": "mongo",
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "securityContext": {
                                            "capabilities": {
                                                "add": [
                                                    "CHOWN",
                                                    "SETGID",
                                                    "SETUID"
                                                ],
                                                "drop": [
                                                    "all"
                                                ]
                                            },
                                            "procMount": "Default",
                                            "readOnlyRootFilesystem": true
                                        },
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File",
                                        "volumeMounts": [
                                            {
                                                "mountPath": "/tmp",
                                                "name": "tmp-volume"
                                            }
                                        ]
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30,
                                "volumes": [
                                    {
                                        "emptyDir": {
                                            "medium": "Memory"
                                        },
                                        "name": "tmp-volume"
                                    }
                                ]
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:49Z",
                                "lastUpdateTime": "2019-04-03T07:35:49Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"payment\"},\"name\":\"payment\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"payment\"}},\"spec\":{\"containers\":[{\"image\":\"weaveworksdemos/payment:0.4.3\",\"name\":\"payment\",\"ports\":[{\"containerPort\":80}],\"securityContext\":{\"capabilities\":{\"add\":[\"NET_BIND_SERVICE\"],\"drop\":[\"all\"]},\"readOnlyRootFilesystem\":true,\"runAsNonRoot\":true,\"runAsUser\":10001}}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"}}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:50Z",
                        "generation": 1,
                        "labels": {
                            "name": "payment"
                        },
                        "name": "payment",
                        "namespace": "sock-shop",
                        "resourceVersion": "1738",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/payment",
                        "uid": "1aa67b8d-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "payment"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "payment"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "image": "weaveworksdemos/payment:0.4.3",
                                        "imagePullPolicy": "IfNotPresent",
                                        "name": "payment",
                                        "ports": [
                                            {
                                                "containerPort": 80,
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "securityContext": {
                                            "capabilities": {
                                                "add": [
                                                    "NET_BIND_SERVICE"
                                                ],
                                                "drop": [
                                                    "all"
                                                ]
                                            },
                                            "procMount": "Default",
                                            "readOnlyRootFilesystem": true,
                                            "runAsNonRoot": true,
                                            "runAsUser": 10001
                                        },
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File"
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:50Z",
                                "lastUpdateTime": "2019-04-03T07:35:50Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"queue-master\"},\"name\":\"queue-master\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"queue-master\"}},\"spec\":{\"containers\":[{\"image\":\"weaveworksdemos/queue-master:0.3.1\",\"name\":\"queue-master\",\"ports\":[{\"containerPort\":80}]}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"}}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:50Z",
                        "generation": 1,
                        "labels": {
                            "name": "queue-master"
                        },
                        "name": "queue-master",
                        "namespace": "sock-shop",
                        "resourceVersion": "2229",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/queue-master",
                        "uid": "1ae3afa6-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "queue-master"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "queue-master"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "image": "weaveworksdemos/queue-master:0.3.1",
                                        "imagePullPolicy": "IfNotPresent",
                                        "name": "queue-master",
                                        "ports": [
                                            {
                                                "containerPort": 80,
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File"
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:51Z",
                                "lastUpdateTime": "2019-04-03T07:35:51Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"rabbitmq\"},\"name\":\"rabbitmq\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"rabbitmq\"}},\"spec\":{\"containers\":[{\"image\":\"rabbitmq:3.6.8\",\"name\":\"rabbitmq\",\"ports\":[{\"containerPort\":5672}],\"securityContext\":{\"capabilities\":{\"add\":[\"CHOWN\",\"SETGID\",\"SETUID\",\"DAC_OVERRIDE\"],\"drop\":[\"all\"]},\"readOnlyRootFilesystem\":true}}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"}}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:51Z",
                        "generation": 1,
                        "labels": {
                            "name": "rabbitmq"
                        },
                        "name": "rabbitmq",
                        "namespace": "sock-shop",
                        "resourceVersion": "1686",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/rabbitmq",
                        "uid": "1b27a832-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "rabbitmq"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "rabbitmq"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "image": "rabbitmq:3.6.8",
                                        "imagePullPolicy": "IfNotPresent",
                                        "name": "rabbitmq",
                                        "ports": [
                                            {
                                                "containerPort": 5672,
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "securityContext": {
                                            "capabilities": {
                                                "add": [
                                                    "CHOWN",
                                                    "SETGID",
                                                    "SETUID",
                                                    "DAC_OVERRIDE"
                                                ],
                                                "drop": [
                                                    "all"
                                                ]
                                            },
                                            "procMount": "Default",
                                            "readOnlyRootFilesystem": true
                                        },
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File"
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:51Z",
                                "lastUpdateTime": "2019-04-03T07:35:51Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"shipping\"},\"name\":\"shipping\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"shipping\"}},\"spec\":{\"containers\":[{\"env\":[{\"name\":\"ZIPKIN\",\"value\":\"zipkin.jaeger.svc.cluster.local\"},{\"name\":\"JAVA_OPTS\",\"value\":\"-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom\"}],\"image\":\"weaveworksdemos/shipping:0.4.8\",\"name\":\"shipping\",\"ports\":[{\"containerPort\":80}],\"securityContext\":{\"capabilities\":{\"add\":[\"NET_BIND_SERVICE\"],\"drop\":[\"all\"]},\"readOnlyRootFilesystem\":true,\"runAsNonRoot\":true,\"runAsUser\":10001},\"volumeMounts\":[{\"mountPath\":\"/tmp\",\"name\":\"tmp-volume\"}]}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"},\"volumes\":[{\"emptyDir\":{\"medium\":\"Memory\"},\"name\":\"tmp-volume\"}]}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:51Z",
                        "generation": 1,
                        "labels": {
                            "name": "shipping"
                        },
                        "name": "shipping",
                        "namespace": "sock-shop",
                        "resourceVersion": "1911",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/shipping",
                        "uid": "1b587463-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "shipping"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "shipping"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "env": [
                                            {
                                                "name": "ZIPKIN",
                                                "value": "zipkin.jaeger.svc.cluster.local"
                                            },
                                            {
                                                "name": "JAVA_OPTS",
                                                "value": "-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom"
                                            }
                                        ],
                                        "image": "weaveworksdemos/shipping:0.4.8",
                                        "imagePullPolicy": "IfNotPresent",
                                        "name": "shipping",
                                        "ports": [
                                            {
                                                "containerPort": 80,
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "securityContext": {
                                            "capabilities": {
                                                "add": [
                                                    "NET_BIND_SERVICE"
                                                ],
                                                "drop": [
                                                    "all"
                                                ]
                                            },
                                            "procMount": "Default",
                                            "readOnlyRootFilesystem": true,
                                            "runAsNonRoot": true,
                                            "runAsUser": 10001
                                        },
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File",
                                        "volumeMounts": [
                                            {
                                                "mountPath": "/tmp",
                                                "name": "tmp-volume"
                                            }
                                        ]
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30,
                                "volumes": [
                                    {
                                        "emptyDir": {
                                            "medium": "Memory"
                                        },
                                        "name": "tmp-volume"
                                    }
                                ]
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:51Z",
                                "lastUpdateTime": "2019-04-03T07:35:51Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"user\"},\"name\":\"user\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"user\"}},\"spec\":{\"containers\":[{\"env\":[{\"name\":\"MONGO_HOST\",\"value\":\"user-db:27017\"}],\"image\":\"weaveworksdemos/user:0.4.7\",\"name\":\"user\",\"ports\":[{\"containerPort\":80}],\"securityContext\":{\"capabilities\":{\"add\":[\"NET_BIND_SERVICE\"],\"drop\":[\"all\"]},\"readOnlyRootFilesystem\":true,\"runAsNonRoot\":true,\"runAsUser\":10001}}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"}}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:52Z",
                        "generation": 1,
                        "labels": {
                            "name": "user"
                        },
                        "name": "user",
                        "namespace": "sock-shop",
                        "resourceVersion": "2374",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/user",
                        "uid": "1bf7878e-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "user"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "user"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "env": [
                                            {
                                                "name": "MONGO_HOST",
                                                "value": "user-db:27017"
                                            }
                                        ],
                                        "image": "weaveworksdemos/user:0.4.7",
                                        "imagePullPolicy": "IfNotPresent",
                                        "name": "user",
                                        "ports": [
                                            {
                                                "containerPort": 80,
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "securityContext": {
                                            "capabilities": {
                                                "add": [
                                                    "NET_BIND_SERVICE"
                                                ],
                                                "drop": [
                                                    "all"
                                                ]
                                            },
                                            "procMount": "Default",
                                            "readOnlyRootFilesystem": true,
                                            "runAsNonRoot": true,
                                            "runAsUser": 10001
                                        },
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File"
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:52Z",
                                "lastUpdateTime": "2019-04-03T07:35:52Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "deployment.kubernetes.io/revision": "1",
                            "kubectl.kubernetes.io/last-applied-configuration": "{\"apiVersion\":\"extensions/v1beta1\",\"kind\":\"Deployment\",\"metadata\":{\"annotations\":{},\"labels\":{\"name\":\"user-db\"},\"name\":\"user-db\",\"namespace\":\"sock-shop\"},\"spec\":{\"replicas\":1,\"template\":{\"metadata\":{\"labels\":{\"name\":\"user-db\"}},\"spec\":{\"containers\":[{\"image\":\"weaveworksdemos/user-db:0.4.0\",\"name\":\"user-db\",\"ports\":[{\"containerPort\":27017,\"name\":\"mongo\"}],\"securityContext\":{\"capabilities\":{\"add\":[\"CHOWN\",\"SETGID\",\"SETUID\"],\"drop\":[\"all\"]},\"readOnlyRootFilesystem\":true},\"volumeMounts\":[{\"mountPath\":\"/tmp\",\"name\":\"tmp-volume\"}]}],\"nodeSelector\":{\"beta.kubernetes.io/os\":\"linux\"},\"volumes\":[{\"emptyDir\":{\"medium\":\"Memory\"},\"name\":\"tmp-volume\"}]}}}}\n"
                        },
                        "creationTimestamp": "2019-04-03T07:35:52Z",
                        "generation": 1,
                        "labels": {
                            "name": "user-db"
                        },
                        "name": "user-db",
                        "namespace": "sock-shop",
                        "resourceVersion": "2061",
                        "selfLink": "/apis/apps/v1/namespaces/sock-shop/deployments/user-db",
                        "uid": "1bae7f07-55e3-11e9-a74e-002481eeda4c"
                    },
                    "spec": {
                        "progressDeadlineSeconds": 2147483647,
                        "replicas": 1,
                        "revisionHistoryLimit": 2147483647,
                        "selector": {
                            "matchLabels": {
                                "name": "user-db"
                            }
                        },
                        "strategy": {
                            "rollingUpdate": {
                                "maxSurge": 1,
                                "maxUnavailable": 1
                            },
                            "type": "RollingUpdate"
                        },
                        "template": {
                            "metadata": {
                                "creationTimestamp": null,
                                "labels": {
                                    "name": "user-db"
                                }
                            },
                            "spec": {
                                "containers": [
                                    {
                                        "image": "weaveworksdemos/user-db:0.4.0",
                                        "imagePullPolicy": "IfNotPresent",
                                        "name": "user-db",
                                        "ports": [
                                            {
                                                "containerPort": 27017,
                                                "name": "mongo",
                                                "protocol": "TCP"
                                            }
                                        ],
                                        "resources": {},
                                        "securityContext": {
                                            "capabilities": {
                                                "add": [
                                                    "CHOWN",
                                                    "SETGID",
                                                    "SETUID"
                                                ],
                                                "drop": [
                                                    "all"
                                                ]
                                            },
                                            "procMount": "Default",
                                            "readOnlyRootFilesystem": true
                                        },
                                        "terminationMessagePath": "/dev/termination-log",
                                        "terminationMessagePolicy": "File",
                                        "volumeMounts": [
                                            {
                                                "mountPath": "/tmp",
                                                "name": "tmp-volume"
                                            }
                                        ]
                                    }
                                ],
                                "dnsPolicy": "ClusterFirst",
                                "nodeSelector": {
                                    "beta.kubernetes.io/os": "linux"
                                },
                                "restartPolicy": "Always",
                                "schedulerName": "default-scheduler",
                                "securityContext": {},
                                "terminationGracePeriodSeconds": 30,
                                "volumes": [
                                    {
                                        "emptyDir": {
                                            "medium": "Memory"
                                        },
                                        "name": "tmp-volume"
                                    }
                                ]
                            }
                        }
                    },
                    "status": {
                        "availableReplicas": 1,
                        "conditions": [
                            {
                                "lastTransitionTime": "2019-04-03T07:35:52Z",
                                "lastUpdateTime": "2019-04-03T07:35:52Z",
                                "message": "Deployment has minimum availability.",
                                "reason": "MinimumReplicasAvailable",
                                "status": "True",
                                "type": "Available"
                            }
                        ],
                        "observedGeneration": 1,
                        "readyReplicas": 1,
                        "replicas": 1,
                        "updatedReplicas": 1
                    }
                }
            ]
        }
    },
    "failed": {},
    "skipped": {},
    "status": {},
    "success": [
        {
            "container_spec": [
                {
                    "env": [
                        {
                            "name": "ZIPKIN",
                            "value": "zipkin.jaeger.svc.cluster.local"
                        },
                        {
                            "name": "JAVA_OPTS",
                            "value": "-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom"
                        }
                    ],
                    "image": "weaveworksdemos/carts:0.4.8",
                    "imagePullPolicy": "IfNotPresent",
                    "name": "carts",
                    "ports": [
                        {
                            "containerPort": 80,
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "securityContext": {
                        "capabilities": {
                            "add": [
                                "NET_BIND_SERVICE"
                            ],
                            "drop": [
                                "all"
                            ]
                        },
                        "procMount": "Default",
                        "readOnlyRootFilesystem": true,
                        "runAsNonRoot": true,
                        "runAsUser": 10001
                    },
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File",
                    "volumeMounts": [
                        {
                            "mountPath": "/tmp",
                            "name": "tmp-volume"
                        }
                    ]
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:48Z",
            "labels": {
                "name": "carts"
            },
            "name": "carts",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "image": "mongo",
                    "imagePullPolicy": "Always",
                    "name": "carts-db",
                    "ports": [
                        {
                            "containerPort": 27017,
                            "name": "mongo",
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "securityContext": {
                        "capabilities": {
                            "add": [
                                "CHOWN",
                                "SETGID",
                                "SETUID"
                            ],
                            "drop": [
                                "all"
                            ]
                        },
                        "procMount": "Default",
                        "readOnlyRootFilesystem": true
                    },
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File",
                    "volumeMounts": [
                        {
                            "mountPath": "/tmp",
                            "name": "tmp-volume"
                        }
                    ]
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:47Z",
            "labels": {
                "name": "carts-db"
            },
            "name": "carts-db",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "image": "weaveworksdemos/catalogue:0.3.5",
                    "imagePullPolicy": "IfNotPresent",
                    "name": "catalogue",
                    "ports": [
                        {
                            "containerPort": 80,
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "securityContext": {
                        "capabilities": {
                            "add": [
                                "NET_BIND_SERVICE"
                            ],
                            "drop": [
                                "all"
                            ]
                        },
                        "procMount": "Default",
                        "readOnlyRootFilesystem": true,
                        "runAsNonRoot": true,
                        "runAsUser": 10001
                    },
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File"
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:48Z",
            "labels": {
                "name": "catalogue"
            },
            "name": "catalogue",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "env": [
                        {
                            "name": "MYSQL_ROOT_PASSWORD",
                            "value": "fake_password"
                        },
                        {
                            "name": "MYSQL_DATABASE",
                            "value": "socksdb"
                        }
                    ],
                    "image": "weaveworksdemos/catalogue-db:0.3.0",
                    "imagePullPolicy": "IfNotPresent",
                    "name": "catalogue-db",
                    "ports": [
                        {
                            "containerPort": 3306,
                            "name": "mysql",
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File"
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:48Z",
            "labels": {
                "name": "catalogue-db"
            },
            "name": "catalogue-db",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "image": "weaveworksdemos/front-end:0.3.12",
                    "imagePullPolicy": "IfNotPresent",
                    "name": "front-end",
                    "ports": [
                        {
                            "containerPort": 8079,
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {
                        "requests": {
                            "cpu": "100m",
                            "memory": "100Mi"
                        }
                    },
                    "securityContext": {
                        "capabilities": {
                            "drop": [
                                "all"
                            ]
                        },
                        "procMount": "Default",
                        "readOnlyRootFilesystem": true,
                        "runAsNonRoot": true,
                        "runAsUser": 10001
                    },
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File"
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:49Z",
            "labels": {
                "name": "front-end"
            },
            "name": "front-end",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "env": [
                        {
                            "name": "ZIPKIN",
                            "value": "zipkin.jaeger.svc.cluster.local"
                        },
                        {
                            "name": "JAVA_OPTS",
                            "value": "-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom"
                        }
                    ],
                    "image": "weaveworksdemos/orders:0.4.7",
                    "imagePullPolicy": "IfNotPresent",
                    "name": "orders",
                    "ports": [
                        {
                            "containerPort": 80,
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "securityContext": {
                        "capabilities": {
                            "add": [
                                "NET_BIND_SERVICE"
                            ],
                            "drop": [
                                "all"
                            ]
                        },
                        "procMount": "Default",
                        "readOnlyRootFilesystem": true,
                        "runAsNonRoot": true,
                        "runAsUser": 10001
                    },
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File",
                    "volumeMounts": [
                        {
                            "mountPath": "/tmp",
                            "name": "tmp-volume"
                        }
                    ]
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:49Z",
            "labels": {
                "name": "orders"
            },
            "name": "orders",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "image": "mongo",
                    "imagePullPolicy": "Always",
                    "name": "orders-db",
                    "ports": [
                        {
                            "containerPort": 27017,
                            "name": "mongo",
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "securityContext": {
                        "capabilities": {
                            "add": [
                                "CHOWN",
                                "SETGID",
                                "SETUID"
                            ],
                            "drop": [
                                "all"
                            ]
                        },
                        "procMount": "Default",
                        "readOnlyRootFilesystem": true
                    },
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File",
                    "volumeMounts": [
                        {
                            "mountPath": "/tmp",
                            "name": "tmp-volume"
                        }
                    ]
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:49Z",
            "labels": {
                "name": "orders-db"
            },
            "name": "orders-db",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "image": "weaveworksdemos/payment:0.4.3",
                    "imagePullPolicy": "IfNotPresent",
                    "name": "payment",
                    "ports": [
                        {
                            "containerPort": 80,
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "securityContext": {
                        "capabilities": {
                            "add": [
                                "NET_BIND_SERVICE"
                            ],
                            "drop": [
                                "all"
                            ]
                        },
                        "procMount": "Default",
                        "readOnlyRootFilesystem": true,
                        "runAsNonRoot": true,
                        "runAsUser": 10001
                    },
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File"
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:50Z",
            "labels": {
                "name": "payment"
            },
            "name": "payment",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "image": "weaveworksdemos/queue-master:0.3.1",
                    "imagePullPolicy": "IfNotPresent",
                    "name": "queue-master",
                    "ports": [
                        {
                            "containerPort": 80,
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File"
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:50Z",
            "labels": {
                "name": "queue-master"
            },
            "name": "queue-master",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "image": "rabbitmq:3.6.8",
                    "imagePullPolicy": "IfNotPresent",
                    "name": "rabbitmq",
                    "ports": [
                        {
                            "containerPort": 5672,
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "securityContext": {
                        "capabilities": {
                            "add": [
                                "CHOWN",
                                "SETGID",
                                "SETUID",
                                "DAC_OVERRIDE"
                            ],
                            "drop": [
                                "all"
                            ]
                        },
                        "procMount": "Default",
                        "readOnlyRootFilesystem": true
                    },
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File"
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:51Z",
            "labels": {
                "name": "rabbitmq"
            },
            "name": "rabbitmq",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "env": [
                        {
                            "name": "ZIPKIN",
                            "value": "zipkin.jaeger.svc.cluster.local"
                        },
                        {
                            "name": "JAVA_OPTS",
                            "value": "-Xms64m -Xmx128m -XX:PermSize=32m -XX:MaxPermSize=64m -XX:+UseG1GC -Djava.security.egd=file:/dev/urandom"
                        }
                    ],
                    "image": "weaveworksdemos/shipping:0.4.8",
                    "imagePullPolicy": "IfNotPresent",
                    "name": "shipping",
                    "ports": [
                        {
                            "containerPort": 80,
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "securityContext": {
                        "capabilities": {
                            "add": [
                                "NET_BIND_SERVICE"
                            ],
                            "drop": [
                                "all"
                            ]
                        },
                        "procMount": "Default",
                        "readOnlyRootFilesystem": true,
                        "runAsNonRoot": true,
                        "runAsUser": 10001
                    },
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File",
                    "volumeMounts": [
                        {
                            "mountPath": "/tmp",
                            "name": "tmp-volume"
                        }
                    ]
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:51Z",
            "labels": {
                "name": "shipping"
            },
            "name": "shipping",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "env": [
                        {
                            "name": "MONGO_HOST",
                            "value": "user-db:27017"
                        }
                    ],
                    "image": "weaveworksdemos/user:0.4.7",
                    "imagePullPolicy": "IfNotPresent",
                    "name": "user",
                    "ports": [
                        {
                            "containerPort": 80,
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "securityContext": {
                        "capabilities": {
                            "add": [
                                "NET_BIND_SERVICE"
                            ],
                            "drop": [
                                "all"
                            ]
                        },
                        "procMount": "Default",
                        "readOnlyRootFilesystem": true,
                        "runAsNonRoot": true,
                        "runAsUser": 10001
                    },
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File"
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:52Z",
            "labels": {
                "name": "user"
            },
            "name": "user",
            "namespace": "sock-shop"
        },
        {
            "container_spec": [
                {
                    "image": "weaveworksdemos/user-db:0.4.0",
                    "imagePullPolicy": "IfNotPresent",
                    "name": "user-db",
                    "ports": [
                        {
                            "containerPort": 27017,
                            "name": "mongo",
                            "protocol": "TCP"
                        }
                    ],
                    "resources": {},
                    "securityContext": {
                        "capabilities": {
                            "add": [
                                "CHOWN",
                                "SETGID",
                                "SETUID"
                            ],
                            "drop": [
                                "all"
                            ]
                        },
                        "procMount": "Default",
                        "readOnlyRootFilesystem": true
                    },
                    "terminationMessagePath": "/dev/termination-log",
                    "terminationMessagePolicy": "File",
                    "volumeMounts": [
                        {
                            "mountPath": "/tmp",
                            "name": "tmp-volume"
                        }
                    ]
                }
            ],
            "creationTimestamp": "2019-04-03T07:35:52Z",
            "labels": {
                "name": "user-db"
            },
            "name": "user-db",
            "namespace": "sock-shop"
        }
    ],
    "unreachable": {}
}
```

#### tool/api/v1.0/get_node

```json
{
    "detail": {
        "10.60.38.181": {
            "_ansible_no_log": false,
            "_ansible_parsed": true,
            "changed": false,
            "invocation": {
                "module_args": {
                    "api_key": null,
                    "api_version": "v1",
                    "cert_file": null,
                    "context": null,
                    "field_selectors": [],
                    "host": null,
                    "key_file": null,
                    "kind": "Node",
                    "kubeconfig": null,
                    "label_selectors": [],
                    "name": null,
                    "namespace": null,
                    "password": null,
                    "ssl_ca_cert": null,
                    "username": null,
                    "verify_ssl": null
                }
            },
            "resources": [
                {
                    "metadata": {
                        "annotations": {
                            "flannel.alpha.coreos.com/backend-data": "{\"VtepMAC\":\"b6:b8:96:f4:04:77\"}",
                            "flannel.alpha.coreos.com/backend-type": "vxlan",
                            "flannel.alpha.coreos.com/kube-subnet-manager": "true",
                            "flannel.alpha.coreos.com/public-ip": "192.168.199.21",
                            "node.alpha.kubernetes.io/ttl": "0",
                            "volumes.kubernetes.io/controller-managed-attach-detach": "true"
                        },
                        "creationTimestamp": "2019-04-03T10:37:38Z",
                        "labels": {
                            "beta.kubernetes.io/arch": "amd64",
                            "beta.kubernetes.io/os": "linux",
                            "kubernetes.io/hostname": "192.168.199.21",
                            "kubernetes.io/role": "master"
                        },
                        "name": "192.168.199.21",
                        "resourceVersion": "697135",
                        "selfLink": "/api/v1/nodes/192.168.199.21",
                        "uid": "800f30f8-55fc-11e9-ba0b-000c29fe0c4c"
                    },
                    "spec": {
                        "podCIDR": "172.20.0.0/24"
                    },
                    "status": {
                        "addresses": [
                            {
                                "address": "192.168.199.21",
                                "type": "InternalIP"
                            },
                            {
                                "address": "192.168.199.21",
                                "type": "Hostname"
                            }
                        ],
                        "allocatable": {
                            "cpu": "2",
                            "ephemeral-storage": "71712187888",
                            "hugepages-1Gi": "0",
                            "hugepages-2Mi": "0",
                            "memory": "8072884Ki",
                            "pods": "110"
                        },
                        "capacity": {
                            "cpu": "2",
                            "ephemeral-storage": "77812704Ki",
                            "hugepages-1Gi": "0",
                            "hugepages-2Mi": "0",
                            "memory": "8175284Ki",
                            "pods": "110"
                        },
                        "conditions": [
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:29Z",
                                "lastTransitionTime": "2019-04-03T10:37:38Z",
                                "message": "kubelet has sufficient disk space available",
                                "reason": "KubeletHasSufficientDisk",
                                "status": "False",
                                "type": "OutOfDisk"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:29Z",
                                "lastTransitionTime": "2019-04-03T10:37:38Z",
                                "message": "kubelet has sufficient memory available",
                                "reason": "KubeletHasSufficientMemory",
                                "status": "False",
                                "type": "MemoryPressure"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:29Z",
                                "lastTransitionTime": "2019-04-03T10:37:38Z",
                                "message": "kubelet has no disk pressure",
                                "reason": "KubeletHasNoDiskPressure",
                                "status": "False",
                                "type": "DiskPressure"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:29Z",
                                "lastTransitionTime": "2019-04-03T10:37:38Z",
                                "message": "kubelet has sufficient PID available",
                                "reason": "KubeletHasSufficientPID",
                                "status": "False",
                                "type": "PIDPressure"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:29Z",
                                "lastTransitionTime": "2019-04-09T06:02:46Z",
                                "message": "kubelet is posting ready status. AppArmor enabled",
                                "reason": "KubeletReady",
                                "status": "True",
                                "type": "Ready"
                            }
                        ],
                        "daemonEndpoints": {
                            "kubeletEndpoint": {
                                "Port": 10250
                            }
                        },
                        "images": [
                            {
                                "names": [
                                    "grafana/grafana@sha256:05d925bd64cd3f9d6f56a4353774ccec588586579ab738f933cd002b7f96aca3",
                                    "grafana/grafana:4.1.2"
                                ],
                                "sizeBytes": 274737916
                            },
                            {
                                "names": [
                                    "weaveworksdemos/orders@sha256:b622e40e83433baf6374f15e076b53893f79958640fc6667dff597622eff03b9",
                                    "weaveworksdemos/orders:0.4.7"
                                ],
                                "sizeBytes": 197650258
                            },
                            {
                                "names": [
                                    "weaveworksdemos/queue-master@sha256:6292d3095f4c7aeed8d863527f8ef6d7a75d3128f20fc61e57f398c100142712",
                                    "weaveworksdemos/queue-master:0.3.1"
                                ],
                                "sizeBytes": 178508575
                            },
                            {
                                "names": [
                                    "jmgao1983/flannel@sha256:bd76b84c74ad70368a2341c2402841b75950df881388e43fc2aca000c546653a",
                                    "jmgao1983/flannel:v0.11.0-amd64"
                                ],
                                "sizeBytes": 52567296
                            },
                            {
                                "names": [
                                    "registry.aliyuncs.com/google_containers/kube-state-metrics@sha256:af98217776f895a280edbf957cccb30b1791145f1cf6fa9822061db30949f369",
                                    "registry.aliyuncs.com/google_containers/kube-state-metrics:v0.4.1"
                                ],
                                "sizeBytes": 45663385
                            },
                            {
                                "names": [
                                    "coredns/coredns@sha256:70a92e9f6fc604f9b629ca331b6135287244a86612f550941193ec7e12759417",
                                    "coredns/coredns:1.4.0"
                                ],
                                "sizeBytes": 42646664
                            },
                            {
                                "names": [
                                    "dockermuenster/caddy@sha256:34899a9cf74fd3943b128e2ce65e08068ec7dcbf3631c5f08c64b483fbf8171b",
                                    "dockermuenster/caddy:0.9.3"
                                ],
                                "sizeBytes": 33210596
                            },
                            {
                                "names": [
                                    "weaveworksdemos/payment@sha256:5ab1c9877480a018d4dda10d6dfa382776e6bca9fc1c60bacbb80903fde8cfe0",
                                    "weaveworksdemos/payment:0.4.3"
                                ],
                                "sizeBytes": 32459351
                            },
                            {
                                "names": [
                                    "giantswarm/tiny-tools@sha256:cc00992e00e14d5c6a502d65822aee048eca08963c66dc21be79efa483a4ef57",
                                    "giantswarm/tiny-tools:latest"
                                ],
                                "sizeBytes": 26606982
                            },
                            {
                                "names": [
                                    "mirrorgooglecontainers/pause-amd64@sha256:59eec8837a4d942cc19a52b8c09ea75121acc38114a2c68b98983ce9356b8610",
                                    "mirrorgooglecontainers/pause-amd64:3.1"
                                ],
                                "sizeBytes": 742472
                            }
                        ],
                        "nodeInfo": {
                            "architecture": "amd64",
                            "bootID": "22a3a311-ec0c-4d1c-aa97-7378e0de9726",
                            "containerRuntimeVersion": "docker://18.9.2",
                            "kernelVersion": "4.4.0-87-generic",
                            "kubeProxyVersion": "v1.12.7",
                            "kubeletVersion": "v1.12.7",
                            "machineID": "c846acdd3c097e1c3d49268b5a6d46ba",
                            "operatingSystem": "linux",
                            "osImage": "Ubuntu 16.04.3 LTS",
                            "systemUUID": "A5174D56-1776-6D13-F1FC-49B226FE0C4C"
                        }
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "flannel.alpha.coreos.com/backend-data": "{\"VtepMAC\":\"0a:07:3a:c7:8d:fa\"}",
                            "flannel.alpha.coreos.com/backend-type": "vxlan",
                            "flannel.alpha.coreos.com/kube-subnet-manager": "true",
                            "flannel.alpha.coreos.com/public-ip": "192.168.199.22",
                            "node.alpha.kubernetes.io/ttl": "0",
                            "volumes.kubernetes.io/controller-managed-attach-detach": "true"
                        },
                        "creationTimestamp": "2019-04-03T10:38:25Z",
                        "labels": {
                            "beta.kubernetes.io/arch": "amd64",
                            "beta.kubernetes.io/os": "linux",
                            "kubernetes.io/hostname": "192.168.199.22",
                            "kubernetes.io/role": "node"
                        },
                        "name": "192.168.199.22",
                        "resourceVersion": "697132",
                        "selfLink": "/api/v1/nodes/192.168.199.22",
                        "uid": "9c32465f-55fc-11e9-ba0b-000c29fe0c4c"
                    },
                    "spec": {
                        "podCIDR": "172.20.2.0/24"
                    },
                    "status": {
                        "addresses": [
                            {
                                "address": "192.168.199.22",
                                "type": "InternalIP"
                            },
                            {
                                "address": "192.168.199.22",
                                "type": "Hostname"
                            }
                        ],
                        "allocatable": {
                            "cpu": "2",
                            "ephemeral-storage": "71712187888",
                            "hugepages-1Gi": "0",
                            "hugepages-2Mi": "0",
                            "memory": "3944116Ki",
                            "pods": "110"
                        },
                        "capacity": {
                            "cpu": "2",
                            "ephemeral-storage": "77812704Ki",
                            "hugepages-1Gi": "0",
                            "hugepages-2Mi": "0",
                            "memory": "4046516Ki",
                            "pods": "110"
                        },
                        "conditions": [
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:27Z",
                                "lastTransitionTime": "2019-04-03T10:38:25Z",
                                "message": "kubelet has sufficient disk space available",
                                "reason": "KubeletHasSufficientDisk",
                                "status": "False",
                                "type": "OutOfDisk"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:27Z",
                                "lastTransitionTime": "2019-04-03T10:38:25Z",
                                "message": "kubelet has sufficient memory available",
                                "reason": "KubeletHasSufficientMemory",
                                "status": "False",
                                "type": "MemoryPressure"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:27Z",
                                "lastTransitionTime": "2019-04-03T10:38:25Z",
                                "message": "kubelet has no disk pressure",
                                "reason": "KubeletHasNoDiskPressure",
                                "status": "False",
                                "type": "DiskPressure"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:27Z",
                                "lastTransitionTime": "2019-04-03T10:38:25Z",
                                "message": "kubelet has sufficient PID available",
                                "reason": "KubeletHasSufficientPID",
                                "status": "False",
                                "type": "PIDPressure"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:27Z",
                                "lastTransitionTime": "2019-04-09T06:02:59Z",
                                "message": "kubelet is posting ready status. AppArmor enabled",
                                "reason": "KubeletReady",
                                "status": "True",
                                "type": "Ready"
                            }
                        ],
                        "daemonEndpoints": {
                            "kubeletEndpoint": {
                                "Port": 10250
                            }
                        },
                        "images": [
                            {
                                "names": [
                                    "mongo@sha256:1dd59670959c3f774c5056e5179145ee9cc06f9003663e14fa44326426a4e6f7",
                                    "mongo:latest"
                                ],
                                "sizeBytes": 409823630
                            },
                            {
                                "names": [
                                    "rabbitmq@sha256:a9f4923559bbcd00b93b02e61615aef5eb6f1d1c98db51053bab0fa6b680db26",
                                    "rabbitmq:3.6.8"
                                ],
                                "sizeBytes": 179449238
                            },
                            {
                                "names": [
                                    "mirrorgooglecontainers/kubernetes-dashboard-amd64@sha256:d6b4e5d77c1cdcb54cd5697a9fe164bc08581a7020d6463986fe1366d36060e8",
                                    "mirrorgooglecontainers/kubernetes-dashboard-amd64:v1.10.1"
                                ],
                                "sizeBytes": 121711221
                            },
                            {
                                "names": [
                                    "prom/prometheus@sha256:e049c086e35c0426389cd2450ef193f6c18b3d0065b97e5f203fdb254716fa1c",
                                    "prom/prometheus:v1.5.2"
                                ],
                                "sizeBytes": 79618077
                            },
                            {
                                "names": [
                                    "jmgao1983/flannel@sha256:bd76b84c74ad70368a2341c2402841b75950df881388e43fc2aca000c546653a",
                                    "jmgao1983/flannel:v0.11.0-amd64"
                                ],
                                "sizeBytes": 52567296
                            },
                            {
                                "names": [
                                    "coredns/coredns@sha256:70a92e9f6fc604f9b629ca331b6135287244a86612f550941193ec7e12759417",
                                    "coredns/coredns:1.4.0"
                                ],
                                "sizeBytes": 42646664
                            },
                            {
                                "names": [
                                    "weaveworksdemos/catalogue@sha256:0147a65b7116569439eefb1a6dbed455fe022464ef70e0c3cab75bc4a226b39b",
                                    "weaveworksdemos/catalogue:0.3.5"
                                ],
                                "sizeBytes": 41221511
                            },
                            {
                                "names": [
                                    "weaveworksdemos/user@sha256:2ffccc332963c89e035fea52201012208bf62df43a55fe461ad6598a5c757ab7",
                                    "weaveworksdemos/user:0.4.7"
                                ],
                                "sizeBytes": 35704702
                            },
                            {
                                "names": [
                                    "dockermuenster/caddy@sha256:34899a9cf74fd3943b128e2ce65e08068ec7dcbf3631c5f08c64b483fbf8171b",
                                    "dockermuenster/caddy:0.9.3"
                                ],
                                "sizeBytes": 33210596
                            },
                            {
                                "names": [
                                    "giantswarm/tiny-tools@sha256:cc00992e00e14d5c6a502d65822aee048eca08963c66dc21be79efa483a4ef57",
                                    "giantswarm/tiny-tools:latest"
                                ],
                                "sizeBytes": 26606982
                            },
                            {
                                "names": [
                                    "mirrorgooglecontainers/pause-amd64@sha256:59eec8837a4d942cc19a52b8c09ea75121acc38114a2c68b98983ce9356b8610",
                                    "mirrorgooglecontainers/pause-amd64:3.1"
                                ],
                                "sizeBytes": 742472
                            }
                        ],
                        "nodeInfo": {
                            "architecture": "amd64",
                            "bootID": "6b77b360-af54-491d-86b1-de32d7c72c46",
                            "containerRuntimeVersion": "docker://18.9.2",
                            "kernelVersion": "4.4.0-87-generic",
                            "kubeProxyVersion": "v1.12.7",
                            "kubeletVersion": "v1.12.7",
                            "machineID": "c846acdd3c097e1c3d49268b5a6d46ba",
                            "operatingSystem": "linux",
                            "osImage": "Ubuntu 16.04.3 LTS",
                            "systemUUID": "36474D56-442C-8B07-83DE-AA04AD45FEFF"
                        }
                    }
                },
                {
                    "metadata": {
                        "annotations": {
                            "flannel.alpha.coreos.com/backend-data": "{\"VtepMAC\":\"92:25:7b:fd:ee:69\"}",
                            "flannel.alpha.coreos.com/backend-type": "vxlan",
                            "flannel.alpha.coreos.com/kube-subnet-manager": "true",
                            "flannel.alpha.coreos.com/public-ip": "192.168.199.23",
                            "node.alpha.kubernetes.io/ttl": "0",
                            "volumes.kubernetes.io/controller-managed-attach-detach": "true"
                        },
                        "creationTimestamp": "2019-04-03T10:38:25Z",
                        "labels": {
                            "beta.kubernetes.io/arch": "amd64",
                            "beta.kubernetes.io/os": "linux",
                            "kubernetes.io/hostname": "192.168.199.23",
                            "kubernetes.io/role": "node"
                        },
                        "name": "192.168.199.23",
                        "resourceVersion": "697129",
                        "selfLink": "/api/v1/nodes/192.168.199.23",
                        "uid": "9c21dbb9-55fc-11e9-ba0b-000c29fe0c4c"
                    },
                    "spec": {
                        "podCIDR": "172.20.1.0/24"
                    },
                    "status": {
                        "addresses": [
                            {
                                "address": "192.168.199.23",
                                "type": "InternalIP"
                            },
                            {
                                "address": "192.168.199.23",
                                "type": "Hostname"
                            }
                        ],
                        "allocatable": {
                            "cpu": "2",
                            "ephemeral-storage": "71712187888",
                            "hugepages-1Gi": "0",
                            "hugepages-2Mi": "0",
                            "memory": "3944116Ki",
                            "pods": "110"
                        },
                        "capacity": {
                            "cpu": "2",
                            "ephemeral-storage": "77812704Ki",
                            "hugepages-1Gi": "0",
                            "hugepages-2Mi": "0",
                            "memory": "4046516Ki",
                            "pods": "110"
                        },
                        "conditions": [
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:26Z",
                                "lastTransitionTime": "2019-04-03T10:38:25Z",
                                "message": "kubelet has sufficient disk space available",
                                "reason": "KubeletHasSufficientDisk",
                                "status": "False",
                                "type": "OutOfDisk"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:26Z",
                                "lastTransitionTime": "2019-04-03T10:38:25Z",
                                "message": "kubelet has sufficient memory available",
                                "reason": "KubeletHasSufficientMemory",
                                "status": "False",
                                "type": "MemoryPressure"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:26Z",
                                "lastTransitionTime": "2019-04-03T10:38:25Z",
                                "message": "kubelet has no disk pressure",
                                "reason": "KubeletHasNoDiskPressure",
                                "status": "False",
                                "type": "DiskPressure"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:26Z",
                                "lastTransitionTime": "2019-04-03T10:38:25Z",
                                "message": "kubelet has sufficient PID available",
                                "reason": "KubeletHasSufficientPID",
                                "status": "False",
                                "type": "PIDPressure"
                            },
                            {
                                "lastHeartbeatTime": "2019-04-09T12:51:26Z",
                                "lastTransitionTime": "2019-04-03T10:38:25Z",
                                "message": "kubelet is posting ready status. AppArmor enabled",
                                "reason": "KubeletReady",
                                "status": "True",
                                "type": "Ready"
                            }
                        ],
                        "daemonEndpoints": {
                            "kubeletEndpoint": {
                                "Port": 10250
                            }
                        },
                        "images": [
                            {
                                "names": [
                                    "weaveworksdemos/user-db@sha256:b43f0f8a76e0c908805fcec74d1ad7f4af4d93c4612632bd6dc20a87508e0b68",
                                    "weaveworksdemos/user-db:0.4.0"
                                ],
                                "sizeBytes": 716879935
                            },
                            {
                                "names": [
                                    "weaveworksdemos/catalogue-db@sha256:7ba74ec9adf88f6625b8d85d3323d1ee5232b39877e1590021ea485cf9457251",
                                    "weaveworksdemos/catalogue-db:0.3.0"
                                ],
                                "sizeBytes": 400161654
                            },
                            {
                                "names": [
                                    "grafana/grafana@sha256:05d925bd64cd3f9d6f56a4353774ccec588586579ab738f933cd002b7f96aca3",
                                    "grafana/grafana:4.1.2"
                                ],
                                "sizeBytes": 274737916
                            },
                            {
                                "names": [
                                    "weaveworksdemos/shipping@sha256:983305c948fded487f4a4acdeab5f898e89d577b4bc1ca3de7750076469ccad4",
                                    "weaveworksdemos/shipping:0.4.8"
                                ],
                                "sizeBytes": 198611718
                            },
                            {
                                "names": [
                                    "weaveworksdemos/carts@sha256:434d2f5a6e0e8beef1f253fe96f45b8437a703125fc003434c5282ecf8969a4f",
                                    "weaveworksdemos/carts:0.4.8"
                                ],
                                "sizeBytes": 197631354
                            },
                            {
                                "names": [
                                    "weaveworksdemos/front-end@sha256:26a2d9b6b291dee2dca32fca3f5bff6c2fa07bb5954359afcbc8001cc70eac71",
                                    "weaveworksdemos/front-end:0.3.12"
                                ],
                                "sizeBytes": 119797603
                            },
                            {
                                "names": [
                                    "prom/prometheus@sha256:e049c086e35c0426389cd2450ef193f6c18b3d0065b97e5f203fdb254716fa1c",
                                    "prom/prometheus:v1.5.2"
                                ],
                                "sizeBytes": 79618077
                            },
                            {
                                "names": [
                                    "mirrorgooglecontainers/heapster-amd64@sha256:3a9d4e2f6d8ee30602bb273b569a5d54e01cce4df152096d150913bc1b9e4968",
                                    "mirrorgooglecontainers/heapster-amd64:v1.5.4"
                                ],
                                "sizeBytes": 75318342
                            },
                            {
                                "names": [
                                    "jmgao1983/flannel@sha256:bd76b84c74ad70368a2341c2402841b75950df881388e43fc2aca000c546653a",
                                    "jmgao1983/flannel:v0.11.0-amd64"
                                ],
                                "sizeBytes": 52567296
                            },
                            {
                                "names": [
                                    "mirrorgooglecontainers/metrics-server-amd64@sha256:ad4a7150389426eedbd2bc81ba8067dc4807b7f47697310a8fe917f34475f83e",
                                    "mirrorgooglecontainers/metrics-server-amd64:v0.3.1"
                                ],
                                "sizeBytes": 40767713
                            },
                            {
                                "names": [
                                    "dockermuenster/caddy@sha256:34899a9cf74fd3943b128e2ce65e08068ec7dcbf3631c5f08c64b483fbf8171b",
                                    "dockermuenster/caddy:0.9.3"
                                ],
                                "sizeBytes": 33210596
                            },
                            {
                                "names": [
                                    "giantswarm/tiny-tools@sha256:cc00992e00e14d5c6a502d65822aee048eca08963c66dc21be79efa483a4ef57",
                                    "giantswarm/tiny-tools:latest"
                                ],
                                "sizeBytes": 26606982
                            },
                            {
                                "names": [
                                    "mirrorgooglecontainers/pause-amd64@sha256:59eec8837a4d942cc19a52b8c09ea75121acc38114a2c68b98983ce9356b8610",
                                    "mirrorgooglecontainers/pause-amd64:3.1"
                                ],
                                "sizeBytes": 742472
                            }
                        ],
                        "nodeInfo": {
                            "architecture": "amd64",
                            "bootID": "eaa20fd6-91ef-44d5-902a-b79541ac34ad",
                            "containerRuntimeVersion": "docker://18.9.2",
                            "kernelVersion": "4.4.0-87-generic",
                            "kubeProxyVersion": "v1.12.7",
                            "kubeletVersion": "v1.12.7",
                            "machineID": "c846acdd3c097e1c3d49268b5a6d46ba",
                            "operatingSystem": "linux",
                            "osImage": "Ubuntu 16.04.3 LTS",
                            "systemUUID": "9B044D56-37A0-A50C-37BF-D0865A8EFAEA"
                        }
                    }
                }
            ]
        }
    },
    "failed": {},
    "skipped": {},
    "status": {},
    "success": [
        {
            "creationTimestamp": "2019-04-03T10:37:38Z",
            "labels": "master",
            "name": "192.168.199.21",
            "uid": "800f30f8-55fc-11e9-ba0b-000c29fe0c4c"
        },
        {
            "creationTimestamp": "2019-04-03T10:38:25Z",
            "labels": "node",
            "name": "192.168.199.22",
            "uid": "9c32465f-55fc-11e9-ba0b-000c29fe0c4c"
        },
        {
            "creationTimestamp": "2019-04-03T10:38:25Z",
            "labels": "node",
            "name": "192.168.199.23",
            "uid": "9c21dbb9-55fc-11e9-ba0b-000c29fe0c4c"
        }
    ],
    "unreachable": {}
}
```

