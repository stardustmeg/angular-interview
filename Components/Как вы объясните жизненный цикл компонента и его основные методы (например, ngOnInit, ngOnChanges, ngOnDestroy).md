
# Жизненные циклы - это последовательность событий, которые происходят в течение жизни компонента. Компоненты в Angular имеют различные жизненные циклы, которые определяют, когда компонент создается, инициализируется, обновляется и уничтожается.

Основные жизненные циклы компонентов в Angular:

1. **Создание компонента**
    
    - Когда Angular создает экземпляр компонента, происходит следующее:
        - Конструктор компонента вызывается.
        - Компонент получает доступ к свойствам и сервисам, которые были предоставлены через инъекцию зависимостей.
        - Если компонент имеет `@Input` свойства, Angular передает значения этих свойств.
2. **Инициализация компонента**
    
    - После создания компонента, Angular вызывает метод `ngOnInit()`. Этот метод  используется для инициализации данных компонента.
3. **Обновление компонента**
    
    - Компонент может быть обновлен, когда изменяются его свойства или данные. Angular вызывает метод `ngOnChanges()`, которыйиспользуется для реагирования на изменения свойств.
4. **Уничтожение компонента**
    
    - Когда компонент больше не нужен, Angular вызывает метод `ngOnDestroy()`. Этот метод используется для очистки ресурсов и освобождения памяти.

Важно отметить, что жизненные циклы компонентов в Angular могут быть дополнены дополнительными методами, такими как `ngAfterViewInit()`, `ngAfterViewChecked()`, `ngDoCheck()` и другие. Эти методы вызываются в различных моментах жизненного цикла компонента и могут быть использованы для выполнения дополнительной логики или реагирования на изменения.