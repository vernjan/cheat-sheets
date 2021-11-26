# Jenkins (Script Console)

## List all jobs without view
To keep it organized

```groovy
def allJobs = Jenkins.instance.getView('all').items.collect {
    it.fullDisplayName
}


def jobsInViews = Jenkins.instance.views
    .findAll { view -> view.name != "all" }
    .collect { view ->
        view.items.collect {
            it.fullDisplayName
        }
    }.flatten()


(allJobs - jobsInViews).each { println it }
```