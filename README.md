Для композиции решил использовать Webpack Module Federation, потому что все микрофронтенды будут на одном React, мне показалось для этого удобнее именно этот метод
Решил разбить на 4 микрофронтенда:
    Host - для композиции всех микрофронтендов

    Places - мф для показа мест, а так же учета лайков, для редактирования мест и загрузки фото. Была мысль развести показ мест и редактирование мест в разные МФ, но мне каежтся это уже создаст сложности и подразумевает взаимодействия между командами работаюищими над этими мф, что плохо скажется на независимости каждой команды.

    Auth - мф для регистрации и логина

    UserProfile - мф для редактирования профиля пользователя
    
В каждом проекте микрофронтенда созданы каталоги components и blocks, для главных компонентов и элементов соотвественно.
МФ Places содержит в себе компонент Main, так как он используется для показа списка мест, что входит в зону отвественности этого микрофронтенда