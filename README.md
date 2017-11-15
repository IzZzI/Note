# Note
AS4.0

1.新的 gradle 插件不再支持 annotation processors，如果需要使用需要显式声明:

 javaCompileOptions {
                includeCompileClasspath = true  
            }
        }
javaCompileOptions {
            annotationProcessorOptions {
                includeCompileClasspath false
            }
        }
