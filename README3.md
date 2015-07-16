#FunsiesSdk

## Table of Contents

<!-- TOC depth:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [FunsiesSdk](#funsiessdk)
	- [Table of Contents](#table-of-contents)
	- [Developing with Grunt](#developing-with-grunt)
		- [Prerequisites](#prerequisites)
		- [Install NodeJS Modules](#install-nodejs-modules)
		- [Build for Production](#build-for-production)
		- [Development](#development)
		- [Automatic Compilation & Testing](#automatic-compilation-testing)
		- [Running Tests](#running-tests)
	- [Setup](#setup)
	- [Authentication:  Login & Logout](#authentication-login-logout)
	- [Using local caching](#using-local-caching)
	- [Models](#models)
		- [Account](#account)
			- [Create](#create)
			- [Update](#update)
			- [Read](#read)
			- [Delete](#delete)
			- [Query Scopes](#query-scopes)
	      
	        
					- [AccountAll](#account-all)
	      
	        
					- [AccountExactMatch](#account-exact-match)
	      
	        
					- [AccountCount](#account-count)
	      
	        
					- [AccountCountExactMatch](#account-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Bird](#bird)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [BirdAll](#bird-all)
	      
	        
					- [BirdExactMatch](#bird-exact-match)
	      
	        
					- [BirdCount](#bird-count)
	      
	        
					- [BirdCountExactMatch](#bird-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Boat](#boat)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [BoatAll](#boat-all)
	      
	        
					- [BoatExactMatch](#boat-exact-match)
	      
	        
					- [BoatCount](#boat-count)
	      
	        
					- [BoatCountExactMatch](#boat-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Car](#car)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [CarAll](#car-all)
	      
	        
					- [CarExactMatch](#car-exact-match)
	      
	        
					- [CarCount](#car-count)
	      
	        
					- [CarCountExactMatch](#car-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Category](#category)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [CategoryAll](#category-all)
	      
	        
					- [CategoryExactMatch](#category-exact-match)
	      
	        
					- [CategoryCount](#category-count)
	      
	        
					- [CategoryCountExactMatch](#category-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Child](#child)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [ChildAll](#child-all)
	      
	        
					- [ChildExactMatch](#child-exact-match)
	      
	        
					- [ChildCount](#child-count)
	      
	        
					- [ChildCountExactMatch](#child-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [City](#city)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [CityAll](#city-all)
	      
	        
					- [CityExactMatch](#city-exact-match)
	      
	        
					- [CityCount](#city-count)
	      
	        
					- [CityCountExactMatch](#city-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Department](#department)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [DepartmentAll](#department-all)
	      
	        
					- [DepartmentExactMatch](#department-exact-match)
	      
	        
					- [DepartmentCount](#department-count)
	      
	        
					- [DepartmentCountExactMatch](#department-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Dog](#dog)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [DogAll](#dog-all)
	      
	        
					- [DogExactMatch](#dog-exact-match)
	      
	        
					- [DogCount](#dog-count)
	      
	        
					- [DogCountExactMatch](#dog-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Dude](#dude)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [DudeAll](#dude-all)
	      
	        
					- [DudeExactMatch](#dude-exact-match)
	      
	        
					- [DudeCount](#dude-count)
	      
	        
					- [DudeCountExactMatch](#dude-count-exact-match)
	      
	        
					- [DudeBooleanAssignableQs](#dude-boolean-assignable-qs)
	      
	        
					- [DudeDateAssignableQs](#dude-date-assignable-qs)
	      
	        
					- [DudeTimeAssignableQs](#dude-time-assignable-qs)
	      
	        
					- [DudeFloatAssignableQs](#dude-float-assignable-qs)
	      
	        
					- [DudeIntegerAssignableQs](#dude-integer-assignable-qs)
	      
	        
					- [DudeStringAssignableQs](#dude-string-assignable-qs)
	      
	        
					- [DudeBooleanDefaultValueQs](#dude-boolean-default-value-qs)
	      
	        
					- [DudeBooleanCountQs](#dude-boolean-count-qs)
	      
	        
					- [DudeDateMinQs](#dude-date-min-qs)
	      
	        
					- [DudeDateMaxQs](#dude-date-max-qs)
	      
	        
					- [DudeDateCountQs](#dude-date-count-qs)
	      
	        
					- [DudeFloatAvgQs](#dude-float-avg-qs)
	      
	        
					- [DudeFloatMinQs](#dude-float-min-qs)
	      
	        
					- [DudeFloatMaxQs](#dude-float-max-qs)
	      
	        
					- [DudeFloatCountQs](#dude-float-count-qs)
	      
	        
					- [DudeFloatSumQs](#dude-float-sum-qs)
	      
	        
					- [DudeIntegerAvgQs](#dude-integer-avg-qs)
	      
	        
					- [DudeIntegerMinQs](#dude-integer-min-qs)
	      
	        
					- [DudeIntegerMaxQs](#dude-integer-max-qs)
	      
	        
					- [DudeIntegerCountQs](#dude-integer-count-qs)
	      
	        
					- [DudeIntegerSumQs](#dude-integer-sum-qs)
	      
	        
					- [DudeStringCountQs](#dude-string-count-qs)
	      
	        
					- [DudeTimeMinQs](#dude-time-min-qs)
	      
	        
					- [DudeTimeMaxQs](#dude-time-max-qs)
	      
	        
					- [DudeTimeCountQs](#dude-time-count-qs)
	      
	        
					- [DudeFloatOpTestQsEq](#dude-float-op-test-qs-eq)
	      
	        
					- [DudeFloatOpTestQsNe](#dude-float-op-test-qs-ne)
	      
	        
					- [DudeFloatOpTestQsGe](#dude-float-op-test-qs-ge)
	      
	        
					- [DudeFloatOpTestQsLe](#dude-float-op-test-qs-le)
	      
	        
					- [DudeFloatOpTestQsGt](#dude-float-op-test-qs-gt)
	      
	        
					- [DudeFloatOpTestQsLt](#dude-float-op-test-qs-lt)
	      
	        
					- [DudeBooleanOpTestQsEq](#dude-boolean-op-test-qs-eq)
	      
	        
					- [DudeBooleanOpTestQsNe](#dude-boolean-op-test-qs-ne)
	      
	        
					- [DudeBooleanOpTestQsGe](#dude-boolean-op-test-qs-ge)
	      
	        
					- [DudeBooleanOpTestQsLe](#dude-boolean-op-test-qs-le)
	      
	        
					- [DudeBooleanOpTestQsGt](#dude-boolean-op-test-qs-gt)
	      
	        
					- [DudeBooleanOpTestQsLt](#dude-boolean-op-test-qs-lt)
	      
	        
					- [DudeIntegerOpTestQsEq](#dude-integer-op-test-qs-eq)
	      
	        
					- [DudeIntegerOpTestQsNe](#dude-integer-op-test-qs-ne)
	      
	        
					- [DudeIntegerOpTestQsGe](#dude-integer-op-test-qs-ge)
	      
	        
					- [DudeIntegerOpTestQsLe](#dude-integer-op-test-qs-le)
	      
	        
					- [DudeIntegerOpTestQsGt](#dude-integer-op-test-qs-gt)
	      
	        
					- [DudeIntegerOpTestQsLt](#dude-integer-op-test-qs-lt)
	      
	        
					- [DudeStringOpTestQsEq](#dude-string-op-test-qs-eq)
	      
	        
					- [DudeStringOpTestQsNe](#dude-string-op-test-qs-ne)
	      
	        
					- [DudeStringOpTestQsGe](#dude-string-op-test-qs-ge)
	      
	        
					- [DudeStringOpTestQsLe](#dude-string-op-test-qs-le)
	      
	        
					- [DudeStringOpTestQsGt](#dude-string-op-test-qs-gt)
	      
	        
					- [DudeStringOpTestQsLt](#dude-string-op-test-qs-lt)
	      
	        
					- [DudeDateOpTestQsEq](#dude-date-op-test-qs-eq)
	      
	        
					- [DudeDateOpTestQsNe](#dude-date-op-test-qs-ne)
	      
	        
					- [DudeDateOpTestQsGe](#dude-date-op-test-qs-ge)
	      
	        
					- [DudeDateOpTestQsLe](#dude-date-op-test-qs-le)
	      
	        
					- [DudeDateOpTestQsGt](#dude-date-op-test-qs-gt)
	      
	        
					- [DudeDateOpTestQsLt](#dude-date-op-test-qs-lt)
	      
	        
					- [DudeTimeOpTestQsEq](#dude-time-op-test-qs-eq)
	      
	        
					- [DudeTimeOpTestQsNe](#dude-time-op-test-qs-ne)
	      
	        
					- [DudeTimeOpTestQsGe](#dude-time-op-test-qs-ge)
	      
	        
					- [DudeTimeOpTestQsLe](#dude-time-op-test-qs-le)
	      
	        
					- [DudeTimeOpTestQsGt](#dude-time-op-test-qs-gt)
	      
	        
					- [DudeTimeOpTestQsLt](#dude-time-op-test-qs-lt)
	      
	        
					- [DudeFloatIgnoreBlankTrueQs](#dude-float-ignore-blank-true-qs)
	      
	        
					- [DudeFloatIgnoreBlankFalseQs](#dude-float-ignore-blank-false-qs)
	      
	        
					- [DudeBooleanIgnoreBlankTrueQs](#dude-boolean-ignore-blank-true-qs)
	      
	        
					- [DudeBooleanIgnoreBlankFalseQs](#dude-boolean-ignore-blank-false-qs)
	      
	        
					- [DudeIntegerIgnoreBlankTrueQs](#dude-integer-ignore-blank-true-qs)
	      
	        
					- [DudeIntegerIgnoreBlankFalseQs](#dude-integer-ignore-blank-false-qs)
	      
	        
					- [DudeStringIgnoreBlankTrueQs](#dude-string-ignore-blank-true-qs)
	      
	        
					- [DudeStringIgnoreBlankFalseQs](#dude-string-ignore-blank-false-qs)
	      
	        
					- [DudeDateIgnoreBlankTrueQs](#dude-date-ignore-blank-true-qs)
	      
	        
					- [DudeDateIgnoreBlankFalseQs](#dude-date-ignore-blank-false-qs)
	      
	        
					- [DudeTimeIgnoreBlankTrueQs](#dude-time-ignore-blank-true-qs)
	      
	        
					- [DudeTimeIgnoreBlankFalseQs](#dude-time-ignore-blank-false-qs)
	      
	        
					- [DudeUserIdQs](#dude-user-id-qs)
	      
	        
					- [DudeCustomObjectQueryScope](#dude-custom-object-query-scope)
	      
	        
					- [DudeParamNameQs](#dude-param-name-qs)
	      
	        
					- [DudeSingleJoinOrQs](#dude-single-join-or-qs)
	      
	        
					- [DudeSingleJoinAndQs](#dude-single-join-and-qs)
	      
	        
					- [DudeMultiJoinQsFirst](#dude-multi-join-qs-first)
	      
	        
					- [DudeMultiJoinQsSecond](#dude-multi-join-qs-second)
	      
	        
					- [DudeMultiJoinQsThird](#dude-multi-join-qs-third)
	      
	        
					- [DudeMultiJoinQsFourth](#dude-multi-join-qs-fourth)
	      
	        
					- [DudeMultiJoinQsFifth](#dude-multi-join-qs-fifth)
	      
	        
					- [DudeTestQs](#dude-test-qs)
	      
	      
	      
	      
    
      
      
        
      
			- [Friend](#friend)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [FriendAll](#friend-all)
	      
	        
					- [FriendExactMatch](#friend-exact-match)
	      
	        
					- [FriendCount](#friend-count)
	      
	        
					- [FriendCountExactMatch](#friend-count-exact-match)
	      
	        
					- [FriendHiddenQs](#friend-hidden-qs)
	      
	      
	      
	      
    
      
      
        
      
			- [Goat](#goat)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [GoatAll](#goat-all)
	      
	        
					- [GoatExactMatch](#goat-exact-match)
	      
	        
					- [GoatCount](#goat-count)
	      
	        
					- [GoatCountExactMatch](#goat-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [House](#house)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [HouseAll](#house-all)
	      
	        
					- [HouseExactMatch](#house-exact-match)
	      
	        
					- [HouseCount](#house-count)
	      
	        
					- [HouseCountExactMatch](#house-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [IncomingContact](#incoming-contact)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [IncomingContactAll](#incoming-contact-all)
	      
	        
					- [IncomingContactExactMatch](#incoming-contact-exact-match)
	      
	        
					- [IncomingContactCount](#incoming-contact-count)
	      
	        
					- [IncomingContactCountExactMatch](#incoming-contact-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Man](#man)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [ManAll](#man-all)
	      
	        
					- [ManExactMatch](#man-exact-match)
	      
	        
					- [ManCount](#man-count)
	      
	        
					- [ManCountExactMatch](#man-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Monkey](#monkey)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [MonkeyAll](#monkey-all)
	      
	        
					- [MonkeyExactMatch](#monkey-exact-match)
	      
	        
					- [MonkeyCount](#monkey-count)
	      
	        
					- [MonkeyCountExactMatch](#monkey-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Order](#order)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [OrderAll](#order-all)
	      
	        
					- [OrderExactMatch](#order-exact-match)
	      
	        
					- [OrderCount](#order-count)
	      
	        
					- [OrderCountExactMatch](#order-count-exact-match)
	      
	        
					- [OrderOrdersInAmountRange](#order-orders-in-amount-range)
	      
	        
					- [OrderPaidOrdersAnd](#order-paid-orders-and)
	      
	        
					- [OrderPaidOrdersOr](#order-paid-orders-or)
	      
	        
					- [OrderCurrentUserOrders](#order-current-user-orders)
	      
	      
	      
	      
    
      
      
        
      
			- [Outage](#outage)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [OutageAll](#outage-all)
	      
	        
					- [OutageExactMatch](#outage-exact-match)
	      
	        
					- [OutageCount](#outage-count)
	      
	        
					- [OutageCountExactMatch](#outage-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Pal](#pal)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [PalAll](#pal-all)
	      
	        
					- [PalExactMatch](#pal-exact-match)
	      
	        
					- [PalCount](#pal-count)
	      
	        
					- [PalCountExactMatch](#pal-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Patient](#patient)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [PatientAll](#patient-all)
	      
	        
					- [PatientExactMatch](#patient-exact-match)
	      
	        
					- [PatientCount](#patient-count)
	      
	        
					- [PatientCountExactMatch](#patient-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Product](#product)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [ProductAll](#product-all)
	      
	        
					- [ProductExactMatch](#product-exact-match)
	      
	        
					- [ProductCount](#product-count)
	      
	        
					- [ProductCountExactMatch](#product-count-exact-match)
	      
	        
					- [ProductSale](#product-sale)
	      
	        
					- [ProductProductsByCategory](#product-products-by-category)
	      
	      
	      
	      
    
      
      
        
      
			- [RelationalDude](#relational-dude)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [RelationalDudeAll](#relational-dude-all)
	      
	        
					- [RelationalDudeExactMatch](#relational-dude-exact-match)
	      
	        
					- [RelationalDudeCount](#relational-dude-count)
	      
	        
					- [RelationalDudeCountExactMatch](#relational-dude-count-exact-match)
	      
	        
					- [RelationalDudeBooleanAssignableQs](#relational-dude-boolean-assignable-qs)
	      
	        
					- [RelationalDudeDateAssignableQs](#relational-dude-date-assignable-qs)
	      
	        
					- [RelationalDudeTimeAssignableQs](#relational-dude-time-assignable-qs)
	      
	        
					- [RelationalDudeFloatAssignableQs](#relational-dude-float-assignable-qs)
	      
	        
					- [RelationalDudeIntegerAssignableQs](#relational-dude-integer-assignable-qs)
	      
	        
					- [RelationalDudeStringAssignableQs](#relational-dude-string-assignable-qs)
	      
	        
					- [RelationalDudeBooleanDefaultValueQs](#relational-dude-boolean-default-value-qs)
	      
	        
					- [RelationalDudeBooleanCountQs](#relational-dude-boolean-count-qs)
	      
	        
					- [RelationalDudeDateMinQs](#relational-dude-date-min-qs)
	      
	        
					- [RelationalDudeDateMaxQs](#relational-dude-date-max-qs)
	      
	        
					- [RelationalDudeDateCountQs](#relational-dude-date-count-qs)
	      
	        
					- [RelationalDudeFloatAvgQs](#relational-dude-float-avg-qs)
	      
	        
					- [RelationalDudeFloatMinQs](#relational-dude-float-min-qs)
	      
	        
					- [RelationalDudeFloatMaxQs](#relational-dude-float-max-qs)
	      
	        
					- [RelationalDudeFloatCountQs](#relational-dude-float-count-qs)
	      
	        
					- [RelationalDudeFloatSumQs](#relational-dude-float-sum-qs)
	      
	        
					- [RelationalDudeIntegerAvgQs](#relational-dude-integer-avg-qs)
	      
	        
					- [RelationalDudeIntegerMinQs](#relational-dude-integer-min-qs)
	      
	        
					- [RelationalDudeIntegerMaxQs](#relational-dude-integer-max-qs)
	      
	        
					- [RelationalDudeIntegerCountQs](#relational-dude-integer-count-qs)
	      
	        
					- [RelationalDudeIntegerSumQs](#relational-dude-integer-sum-qs)
	      
	        
					- [RelationalDudeStringCountQs](#relational-dude-string-count-qs)
	      
	        
					- [RelationalDudeTimeMinQs](#relational-dude-time-min-qs)
	      
	        
					- [RelationalDudeTimeMaxQs](#relational-dude-time-max-qs)
	      
	        
					- [RelationalDudeTimeCountQs](#relational-dude-time-count-qs)
	      
	        
					- [RelationalDudeFloatOpTestQsEq](#relational-dude-float-op-test-qs-eq)
	      
	        
					- [RelationalDudeFloatOpTestQsNe](#relational-dude-float-op-test-qs-ne)
	      
	        
					- [RelationalDudeFloatOpTestQsGe](#relational-dude-float-op-test-qs-ge)
	      
	        
					- [RelationalDudeFloatOpTestQsLe](#relational-dude-float-op-test-qs-le)
	      
	        
					- [RelationalDudeFloatOpTestQsGt](#relational-dude-float-op-test-qs-gt)
	      
	        
					- [RelationalDudeFloatOpTestQsLt](#relational-dude-float-op-test-qs-lt)
	      
	        
					- [RelationalDudeBooleanOpTestQsEq](#relational-dude-boolean-op-test-qs-eq)
	      
	        
					- [RelationalDudeBooleanOpTestQsNe](#relational-dude-boolean-op-test-qs-ne)
	      
	        
					- [RelationalDudeBooleanOpTestQsGe](#relational-dude-boolean-op-test-qs-ge)
	      
	        
					- [RelationalDudeBooleanOpTestQsLe](#relational-dude-boolean-op-test-qs-le)
	      
	        
					- [RelationalDudeBooleanOpTestQsGt](#relational-dude-boolean-op-test-qs-gt)
	      
	        
					- [RelationalDudeBooleanOpTestQsLt](#relational-dude-boolean-op-test-qs-lt)
	      
	        
					- [RelationalDudeIntegerOpTestQsEq](#relational-dude-integer-op-test-qs-eq)
	      
	        
					- [RelationalDudeIntegerOpTestQsNe](#relational-dude-integer-op-test-qs-ne)
	      
	        
					- [RelationalDudeIntegerOpTestQsGe](#relational-dude-integer-op-test-qs-ge)
	      
	        
					- [RelationalDudeIntegerOpTestQsLe](#relational-dude-integer-op-test-qs-le)
	      
	        
					- [RelationalDudeIntegerOpTestQsGt](#relational-dude-integer-op-test-qs-gt)
	      
	        
					- [RelationalDudeIntegerOpTestQsLt](#relational-dude-integer-op-test-qs-lt)
	      
	        
					- [RelationalDudeStringOpTestQsEq](#relational-dude-string-op-test-qs-eq)
	      
	        
					- [RelationalDudeStringOpTestQsNe](#relational-dude-string-op-test-qs-ne)
	      
	        
					- [RelationalDudeStringOpTestQsGe](#relational-dude-string-op-test-qs-ge)
	      
	        
					- [RelationalDudeStringOpTestQsLe](#relational-dude-string-op-test-qs-le)
	      
	        
					- [RelationalDudeStringOpTestQsGt](#relational-dude-string-op-test-qs-gt)
	      
	        
					- [RelationalDudeStringOpTestQsLt](#relational-dude-string-op-test-qs-lt)
	      
	        
					- [RelationalDudeDateOpTestQsEq](#relational-dude-date-op-test-qs-eq)
	      
	        
					- [RelationalDudeDateOpTestQsNe](#relational-dude-date-op-test-qs-ne)
	      
	        
					- [RelationalDudeDateOpTestQsGe](#relational-dude-date-op-test-qs-ge)
	      
	        
					- [RelationalDudeDateOpTestQsLe](#relational-dude-date-op-test-qs-le)
	      
	        
					- [RelationalDudeDateOpTestQsGt](#relational-dude-date-op-test-qs-gt)
	      
	        
					- [RelationalDudeDateOpTestQsLt](#relational-dude-date-op-test-qs-lt)
	      
	        
					- [RelationalDudeTimeOpTestQsEq](#relational-dude-time-op-test-qs-eq)
	      
	        
					- [RelationalDudeTimeOpTestQsNe](#relational-dude-time-op-test-qs-ne)
	      
	        
					- [RelationalDudeTimeOpTestQsGe](#relational-dude-time-op-test-qs-ge)
	      
	        
					- [RelationalDudeTimeOpTestQsLe](#relational-dude-time-op-test-qs-le)
	      
	        
					- [RelationalDudeTimeOpTestQsGt](#relational-dude-time-op-test-qs-gt)
	      
	        
					- [RelationalDudeTimeOpTestQsLt](#relational-dude-time-op-test-qs-lt)
	      
	        
					- [RelationalDudeFloatIgnoreBlankTrueQs](#relational-dude-float-ignore-blank-true-qs)
	      
	        
					- [RelationalDudeFloatIgnoreBlankFalseQs](#relational-dude-float-ignore-blank-false-qs)
	      
	        
					- [RelationalDudeBooleanIgnoreBlankTrueQs](#relational-dude-boolean-ignore-blank-true-qs)
	      
	        
					- [RelationalDudeBooleanIgnoreBlankFalseQs](#relational-dude-boolean-ignore-blank-false-qs)
	      
	        
					- [RelationalDudeIntegerIgnoreBlankTrueQs](#relational-dude-integer-ignore-blank-true-qs)
	      
	        
					- [RelationalDudeIntegerIgnoreBlankFalseQs](#relational-dude-integer-ignore-blank-false-qs)
	      
	        
					- [RelationalDudeStringIgnoreBlankTrueQs](#relational-dude-string-ignore-blank-true-qs)
	      
	        
					- [RelationalDudeStringIgnoreBlankFalseQs](#relational-dude-string-ignore-blank-false-qs)
	      
	        
					- [RelationalDudeDateIgnoreBlankTrueQs](#relational-dude-date-ignore-blank-true-qs)
	      
	        
					- [RelationalDudeDateIgnoreBlankFalseQs](#relational-dude-date-ignore-blank-false-qs)
	      
	        
					- [RelationalDudeTimeIgnoreBlankTrueQs](#relational-dude-time-ignore-blank-true-qs)
	      
	        
					- [RelationalDudeTimeIgnoreBlankFalseQs](#relational-dude-time-ignore-blank-false-qs)
	      
	        
					- [RelationalDudeUserIdQs](#relational-dude-user-id-qs)
	      
	        
					- [RelationalDudeCustomObjectQueryScope](#relational-dude-custom-object-query-scope)
	      
	        
					- [RelationalDudeParamNameQs](#relational-dude-param-name-qs)
	      
	        
					- [RelationalDudeSingleJoinOrQs](#relational-dude-single-join-or-qs)
	      
	        
					- [RelationalDudeSingleJoinAndQs](#relational-dude-single-join-and-qs)
	      
	        
					- [RelationalDudeMultiJoinQsFirst](#relational-dude-multi-join-qs-first)
	      
	        
					- [RelationalDudeMultiJoinQsSecond](#relational-dude-multi-join-qs-second)
	      
	        
					- [RelationalDudeMultiJoinQsThird](#relational-dude-multi-join-qs-third)
	      
	        
					- [RelationalDudeMultiJoinQsFourth](#relational-dude-multi-join-qs-fourth)
	      
	        
					- [RelationalDudeMultiJoinQsFifth](#relational-dude-multi-join-qs-fifth)
	      
	        
					- [RelationalDudeTestQs](#relational-dude-test-qs)
	      
	      
	      
	      
    
      
      
        
      
			- [Restaurant](#restaurant)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [RestaurantAll](#restaurant-all)
	      
	        
					- [RestaurantExactMatch](#restaurant-exact-match)
	      
	        
					- [RestaurantCount](#restaurant-count)
	      
	        
					- [RestaurantCountExactMatch](#restaurant-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Robot](#robot)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [RobotAll](#robot-all)
	      
	        
					- [RobotExactMatch](#robot-exact-match)
	      
	        
					- [RobotCount](#robot-count)
	      
	        
					- [RobotCountExactMatch](#robot-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [SalesReport](#sales-report)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [SalesReportAll](#sales-report-all)
	      
	        
					- [SalesReportExactMatch](#sales-report-exact-match)
	      
	        
					- [SalesReportCount](#sales-report-count)
	      
	        
					- [SalesReportCountExactMatch](#sales-report-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [SalesforceAccount](#salesforce-account)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [SalesforceAccountAll](#salesforce-account-all)
	      
	        
					- [SalesforceAccountExactMatch](#salesforce-account-exact-match)
	      
	        
					- [SalesforceAccountCount](#salesforce-account-count)
	      
	        
					- [SalesforceAccountCountExactMatch](#salesforce-account-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [SalesforceContact](#salesforce-contact)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [SalesforceContactAll](#salesforce-contact-all)
	      
	        
					- [SalesforceContactExactMatch](#salesforce-contact-exact-match)
	      
	        
					- [SalesforceContactCount](#salesforce-contact-count)
	      
	        
					- [SalesforceContactCountExactMatch](#salesforce-contact-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Store](#store)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [StoreAll](#store-all)
	      
	        
					- [StoreExactMatch](#store-exact-match)
	      
	        
					- [StoreCount](#store-count)
	      
	        
					- [StoreCountExactMatch](#store-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Subscriber](#subscriber)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [SubscriberAll](#subscriber-all)
	      
	        
					- [SubscriberExactMatch](#subscriber-exact-match)
	      
	        
					- [SubscriberCount](#subscriber-count)
	      
	        
					- [SubscriberCountExactMatch](#subscriber-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [User](#user)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [UserAll](#user-all)
	      
	        
					- [UserExactMatch](#user-exact-match)
	      
	        
					- [UserCount](#user-count)
	      
	        
					- [UserCountExactMatch](#user-count-exact-match)
	      
	      
	      
	      
    
      
      
        
      
			- [Wizard](#wizard)
				- [Create](#create-#{index-1})
				- [Update](#update-#{index-1})
				- [Read](#read-#{index-1})
				- [Delete](#delete-#{index-1})
				- [Query Scopes](#query-scopes-#{index-1})
	      
	        
					- [WizardAll](#wizard-all)
	      
	        
					- [WizardExactMatch](#wizard-exact-match)
	      
	        
					- [WizardCount](#wizard-count)
	      
	        
					- [WizardCountExactMatch](#wizard-count-exact-match)
	      
	      
	      
	      
    
<!-- /TOC -->

## Developing with Grunt

Grunt is a NodeJS-based task runner.  It helps automate common tasks, such as
asset compilation, minification, and testing.  Grunt tasks are included for this
SDK in `Gruntfile.js`.

Follow directions below to get up and running with Grunt.

### Prerequisites

- [NodeJS](http://nodejs.org)

### Install NodeJS Modules

From the root directory of the SDK (where `Gruntfile.js` is
located), install NodeJS modules:

    npm install

### Build for Production

To compile assets and create a full production build, run the
build task:

    grunt build

### Development

During development, a full minified SDK build is unnecessary.  To
compile assets without minifying:

    grunt compile

### Automatic Compilation & Testing

Since it's cumbersome to manually compile assets after every change during
development, the SDK's `Gruntfile.js` includes a `watch` task.  The
task monitors changes to the SDK's `coffee` and `sass` assets,
automatically compiling (but not minifying) them.  Run the following command
before making changes:

    grunt watch

SDK tests are also executed by the `watch` task.  If changing the SDK
significantly, some or all tests may fail.  You may disable auto-testing by
editing the `watch` task in `Gruntfile.js`.

### Running Tests

The SDK comes with a complete test suite.  Execute tests from grunt:

    grunt test

Or execute tests directly in a browser.  Open `test/index.html` and click
"Run Tests".

##Setup

To initialize the SDK you must first provide a base URL for your backend server. Then, all you need to do is call the init method on FunsiesSdk.

```javascript
FunsiesSdk.baseUrl = "https://www.foo.com";
FunsiesSdk.init();
```

If your application is *DirectToSource* then you can skip the base URL setup.

## Authentication:  Login & Logout
```javascript
AP.auth.Authentication.login({
  username: 'test',
  password: 'password'
});

AP.auth.Authentication.logout();
```

##Using local caching

Local caching can be toggled easily by setting the value of the Application variable `useOfflineCache` **before** initializing the SDK.

```javascript
FunsiesSdk.useOfflineCache = true;
FunsiesSdk.init();
```

If you would like to activate it **after** initialization, you can use the method `initOfflineCache` on the SDK.

```javascript
FunsiesSdk.initOfflineCache();
```

Keep in mind that once local caching has been enabled it cannot be disabled in runtime.

##Models

Available Model objects:

* Account
* Bird
* Boat
* Car
* Category
* Child
* City
* Department
* Dog
* Dude
* Friend
* Goat
* House
* IncomingContact
* Man
* Monkey
* Order
* Outage
* Pal
* Patient
* Product
* RelationalDude
* Restaurant
* Robot
* SalesReport
* SalesforceAccount
* SalesforceContact
* Store
* Subscriber
* User
* Wizard

###Account

####Create

This is an example of how you would create a Account Model.

```javascript
var exampleModel = new FunsiesSdk.models.Account();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Account Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Account instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Account({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Account objects are:

* AccountAll
* AccountExactMatch
* AccountCount
* AccountCountExactMatch

#####AccountAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var AccountAll = new FunsiesSdk.collections.AccountAll();

// using the query method
AccountAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
AccountAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
AccountAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####AccountExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var AccountExactMatch = new FunsiesSdk.collections.AccountExactMatch();

// using the query method
AccountExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
AccountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
AccountExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####AccountCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var AccountCount = new FunsiesSdk.collections.AccountCount();

// using the query method
AccountCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
AccountCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = AccountCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
AccountCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = AccountCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####AccountCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var AccountCountExactMatch = new FunsiesSdk.collections.AccountCountExactMatch();

// using the query method
AccountCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
AccountCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = AccountCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
AccountCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = AccountCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Bird

####Create

This is an example of how you would create a Bird Model.

```javascript
var exampleModel = new FunsiesSdk.models.Bird();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Bird Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Bird instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Bird({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Bird objects are:

* BirdAll
* BirdExactMatch
* BirdCount
* BirdCountExactMatch

#####BirdAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var BirdAll = new FunsiesSdk.collections.BirdAll();

// using the query method
BirdAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
BirdAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
BirdAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####BirdExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var BirdExactMatch = new FunsiesSdk.collections.BirdExactMatch();

// using the query method
BirdExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
BirdExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
BirdExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####BirdCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var BirdCount = new FunsiesSdk.collections.BirdCount();

// using the query method
BirdCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
BirdCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = BirdCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
BirdCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = BirdCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####BirdCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var BirdCountExactMatch = new FunsiesSdk.collections.BirdCountExactMatch();

// using the query method
BirdCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
BirdCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = BirdCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
BirdCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = BirdCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Boat

####Create

This is an example of how you would create a Boat Model.

```javascript
var exampleModel = new FunsiesSdk.models.Boat();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Boat Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Boat instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Boat({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Boat objects are:

* BoatAll
* BoatExactMatch
* BoatCount
* BoatCountExactMatch

#####BoatAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var BoatAll = new FunsiesSdk.collections.BoatAll();

// using the query method
BoatAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
BoatAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
BoatAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####BoatExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var BoatExactMatch = new FunsiesSdk.collections.BoatExactMatch();

// using the query method
BoatExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
BoatExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
BoatExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####BoatCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var BoatCount = new FunsiesSdk.collections.BoatCount();

// using the query method
BoatCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
BoatCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = BoatCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
BoatCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = BoatCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####BoatCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var BoatCountExactMatch = new FunsiesSdk.collections.BoatCountExactMatch();

// using the query method
BoatCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
BoatCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = BoatCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
BoatCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = BoatCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Car

####Create

This is an example of how you would create a Car Model.

```javascript
var exampleModel = new FunsiesSdk.models.Car();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Car Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Car instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Car({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Car objects are:

* CarAll
* CarExactMatch
* CarCount
* CarCountExactMatch

#####CarAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CarAll = new FunsiesSdk.collections.CarAll();

// using the query method
CarAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CarAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CarAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####CarExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CarExactMatch = new FunsiesSdk.collections.CarExactMatch();

// using the query method
CarExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CarExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CarExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####CarCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CarCount = new FunsiesSdk.collections.CarCount();

// using the query method
CarCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CarCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = CarCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CarCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = CarCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####CarCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CarCountExactMatch = new FunsiesSdk.collections.CarCountExactMatch();

// using the query method
CarCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CarCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = CarCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CarCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = CarCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Category

####Create

This is an example of how you would create a Category Model.

```javascript
var exampleModel = new FunsiesSdk.models.Category();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Category Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Category instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Category({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Category objects are:

* CategoryAll
* CategoryExactMatch
* CategoryCount
* CategoryCountExactMatch

#####CategoryAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CategoryAll = new FunsiesSdk.collections.CategoryAll();

// using the query method
CategoryAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CategoryAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CategoryAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####CategoryExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CategoryExactMatch = new FunsiesSdk.collections.CategoryExactMatch();

// using the query method
CategoryExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CategoryExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CategoryExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####CategoryCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CategoryCount = new FunsiesSdk.collections.CategoryCount();

// using the query method
CategoryCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CategoryCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = CategoryCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CategoryCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = CategoryCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####CategoryCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CategoryCountExactMatch = new FunsiesSdk.collections.CategoryCountExactMatch();

// using the query method
CategoryCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CategoryCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = CategoryCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CategoryCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = CategoryCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Child

####Create

This is an example of how you would create a Child Model.

```javascript
var exampleModel = new FunsiesSdk.models.Child();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Child Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Child instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Child({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Child objects are:

* ChildAll
* ChildExactMatch
* ChildCount
* ChildCountExactMatch

#####ChildAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ChildAll = new FunsiesSdk.collections.ChildAll();

// using the query method
ChildAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ChildAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ChildAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####ChildExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ChildExactMatch = new FunsiesSdk.collections.ChildExactMatch();

// using the query method
ChildExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ChildExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ChildExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####ChildCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ChildCount = new FunsiesSdk.collections.ChildCount();

// using the query method
ChildCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ChildCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = ChildCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ChildCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = ChildCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####ChildCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ChildCountExactMatch = new FunsiesSdk.collections.ChildCountExactMatch();

// using the query method
ChildCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ChildCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = ChildCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ChildCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = ChildCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###City

####Create

This is an example of how you would create a City Model.

```javascript
var exampleModel = new FunsiesSdk.models.City();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a City Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single City instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.City({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for City objects are:

* CityAll
* CityExactMatch
* CityCount
* CityCountExactMatch

#####CityAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CityAll = new FunsiesSdk.collections.CityAll();

// using the query method
CityAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CityAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CityAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####CityExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CityExactMatch = new FunsiesSdk.collections.CityExactMatch();

// using the query method
CityExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CityExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CityExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####CityCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CityCount = new FunsiesSdk.collections.CityCount();

// using the query method
CityCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CityCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = CityCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CityCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = CityCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####CityCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var CityCountExactMatch = new FunsiesSdk.collections.CityCountExactMatch();

// using the query method
CityCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
CityCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = CityCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
CityCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = CityCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Department

####Create

This is an example of how you would create a Department Model.

```javascript
var exampleModel = new FunsiesSdk.models.Department();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Department Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Department instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Department({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Department objects are:

* DepartmentAll
* DepartmentExactMatch
* DepartmentCount
* DepartmentCountExactMatch

#####DepartmentAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DepartmentAll = new FunsiesSdk.collections.DepartmentAll();

// using the query method
DepartmentAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DepartmentAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DepartmentAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DepartmentExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DepartmentExactMatch = new FunsiesSdk.collections.DepartmentExactMatch();

// using the query method
DepartmentExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DepartmentExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DepartmentExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DepartmentCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DepartmentCount = new FunsiesSdk.collections.DepartmentCount();

// using the query method
DepartmentCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DepartmentCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DepartmentCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DepartmentCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DepartmentCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DepartmentCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DepartmentCountExactMatch = new FunsiesSdk.collections.DepartmentCountExactMatch();

// using the query method
DepartmentCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DepartmentCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DepartmentCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DepartmentCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DepartmentCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Dog

####Create

This is an example of how you would create a Dog Model.

```javascript
var exampleModel = new FunsiesSdk.models.Dog();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Dog Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Dog instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Dog({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Dog objects are:

* DogAll
* DogExactMatch
* DogCount
* DogCountExactMatch

#####DogAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DogAll = new FunsiesSdk.collections.DogAll();

// using the query method
DogAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DogAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DogAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DogExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DogExactMatch = new FunsiesSdk.collections.DogExactMatch();

// using the query method
DogExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DogExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DogExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DogCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DogCount = new FunsiesSdk.collections.DogCount();

// using the query method
DogCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DogCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DogCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DogCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DogCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DogCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DogCountExactMatch = new FunsiesSdk.collections.DogCountExactMatch();

// using the query method
DogCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DogCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DogCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DogCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DogCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Dude

####Create

This is an example of how you would create a Dude Model.

```javascript
var exampleModel = new FunsiesSdk.models.Dude();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Dude Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Dude instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Dude({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Dude objects are:

* DudeAll
* DudeExactMatch
* DudeCount
* DudeCountExactMatch
* DudeBooleanAssignableQs
* DudeDateAssignableQs
* DudeTimeAssignableQs
* DudeFloatAssignableQs
* DudeIntegerAssignableQs
* DudeStringAssignableQs
* DudeBooleanDefaultValueQs
* DudeBooleanCountQs
* DudeDateMinQs
* DudeDateMaxQs
* DudeDateCountQs
* DudeFloatAvgQs
* DudeFloatMinQs
* DudeFloatMaxQs
* DudeFloatCountQs
* DudeFloatSumQs
* DudeIntegerAvgQs
* DudeIntegerMinQs
* DudeIntegerMaxQs
* DudeIntegerCountQs
* DudeIntegerSumQs
* DudeStringCountQs
* DudeTimeMinQs
* DudeTimeMaxQs
* DudeTimeCountQs
* DudeFloatOpTestQsEq
* DudeFloatOpTestQsNe
* DudeFloatOpTestQsGe
* DudeFloatOpTestQsLe
* DudeFloatOpTestQsGt
* DudeFloatOpTestQsLt
* DudeBooleanOpTestQsEq
* DudeBooleanOpTestQsNe
* DudeBooleanOpTestQsGe
* DudeBooleanOpTestQsLe
* DudeBooleanOpTestQsGt
* DudeBooleanOpTestQsLt
* DudeIntegerOpTestQsEq
* DudeIntegerOpTestQsNe
* DudeIntegerOpTestQsGe
* DudeIntegerOpTestQsLe
* DudeIntegerOpTestQsGt
* DudeIntegerOpTestQsLt
* DudeStringOpTestQsEq
* DudeStringOpTestQsNe
* DudeStringOpTestQsGe
* DudeStringOpTestQsLe
* DudeStringOpTestQsGt
* DudeStringOpTestQsLt
* DudeDateOpTestQsEq
* DudeDateOpTestQsNe
* DudeDateOpTestQsGe
* DudeDateOpTestQsLe
* DudeDateOpTestQsGt
* DudeDateOpTestQsLt
* DudeTimeOpTestQsEq
* DudeTimeOpTestQsNe
* DudeTimeOpTestQsGe
* DudeTimeOpTestQsLe
* DudeTimeOpTestQsGt
* DudeTimeOpTestQsLt
* DudeFloatIgnoreBlankTrueQs
* DudeFloatIgnoreBlankFalseQs
* DudeBooleanIgnoreBlankTrueQs
* DudeBooleanIgnoreBlankFalseQs
* DudeIntegerIgnoreBlankTrueQs
* DudeIntegerIgnoreBlankFalseQs
* DudeStringIgnoreBlankTrueQs
* DudeStringIgnoreBlankFalseQs
* DudeDateIgnoreBlankTrueQs
* DudeDateIgnoreBlankFalseQs
* DudeTimeIgnoreBlankTrueQs
* DudeTimeIgnoreBlankFalseQs
* DudeUserIdQs
* DudeCustomObjectQueryScope
* DudeParamNameQs
* DudeSingleJoinOrQs
* DudeSingleJoinAndQs
* DudeMultiJoinQsFirst
* DudeMultiJoinQsSecond
* DudeMultiJoinQsThird
* DudeMultiJoinQsFourth
* DudeMultiJoinQsFifth
* DudeTestQs

#####DudeAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeAll = new FunsiesSdk.collections.DudeAll();

// using the query method
DudeAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeExactMatch = new FunsiesSdk.collections.DudeExactMatch();

// using the query method
DudeExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeCount = new FunsiesSdk.collections.DudeCount();

// using the query method
DudeCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeCountExactMatch = new FunsiesSdk.collections.DudeCountExactMatch();

// using the query method
DudeCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeBooleanAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeBooleanAssignableQs = new FunsiesSdk.collections.DudeBooleanAssignableQs();

// using the query method
DudeBooleanAssignableQs.query({
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeBooleanAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeBooleanAssignableQs.query({
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeDateAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateAssignableQs = new FunsiesSdk.collections.DudeDateAssignableQs();

// using the query method
DudeDateAssignableQs.query({
  
  "my_date": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_date": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateAssignableQs.query({
  
  "my_date": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeTimeAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeAssignableQs = new FunsiesSdk.collections.DudeTimeAssignableQs();

// using the query method
DudeTimeAssignableQs.query({
  
  "my_time": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_time": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeAssignableQs.query({
  
  "my_time": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeFloatAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatAssignableQs = new FunsiesSdk.collections.DudeFloatAssignableQs();

// using the query method
DudeFloatAssignableQs.query({
  
  "my_float": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_float": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatAssignableQs.query({
  
  "my_float": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeIntegerAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerAssignableQs = new FunsiesSdk.collections.DudeIntegerAssignableQs();

// using the query method
DudeIntegerAssignableQs.query({
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerAssignableQs.query({
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeStringAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeStringAssignableQs = new FunsiesSdk.collections.DudeStringAssignableQs();

// using the query method
DudeStringAssignableQs.query({
  
  "my_string": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeStringAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeStringAssignableQs.query({
  
  "my_string": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeBooleanDefaultValueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeBooleanDefaultValueQs = new FunsiesSdk.collections.DudeBooleanDefaultValueQs();

// using the query method
DudeBooleanDefaultValueQs.query({
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeBooleanDefaultValueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeBooleanDefaultValueQs.query({
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeBooleanCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeBooleanCountQs = new FunsiesSdk.collections.DudeBooleanCountQs();

// using the query method
DudeBooleanCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeBooleanCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeBooleanCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeBooleanCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeBooleanCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeDateMinQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateMinQs = new FunsiesSdk.collections.DudeDateMinQs();

// using the query method
DudeDateMinQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateMinQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeDateMinQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateMinQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeDateMinQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeDateMaxQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateMaxQs = new FunsiesSdk.collections.DudeDateMaxQs();

// using the query method
DudeDateMaxQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateMaxQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeDateMaxQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateMaxQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeDateMaxQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeDateCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateCountQs = new FunsiesSdk.collections.DudeDateCountQs();

// using the query method
DudeDateCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeDateCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeDateCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeFloatAvgQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatAvgQs = new FunsiesSdk.collections.DudeFloatAvgQs();

// using the query method
DudeFloatAvgQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatAvgQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeFloatAvgQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatAvgQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeFloatAvgQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeFloatMinQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatMinQs = new FunsiesSdk.collections.DudeFloatMinQs();

// using the query method
DudeFloatMinQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatMinQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeFloatMinQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatMinQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeFloatMinQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeFloatMaxQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatMaxQs = new FunsiesSdk.collections.DudeFloatMaxQs();

// using the query method
DudeFloatMaxQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatMaxQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeFloatMaxQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatMaxQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeFloatMaxQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeFloatCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatCountQs = new FunsiesSdk.collections.DudeFloatCountQs();

// using the query method
DudeFloatCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeFloatCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeFloatCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeFloatSumQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatSumQs = new FunsiesSdk.collections.DudeFloatSumQs();

// using the query method
DudeFloatSumQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatSumQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeFloatSumQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatSumQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeFloatSumQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeIntegerAvgQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerAvgQs = new FunsiesSdk.collections.DudeIntegerAvgQs();

// using the query method
DudeIntegerAvgQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerAvgQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeIntegerAvgQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerAvgQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeIntegerAvgQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeIntegerMinQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerMinQs = new FunsiesSdk.collections.DudeIntegerMinQs();

// using the query method
DudeIntegerMinQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerMinQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeIntegerMinQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerMinQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeIntegerMinQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeIntegerMaxQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerMaxQs = new FunsiesSdk.collections.DudeIntegerMaxQs();

// using the query method
DudeIntegerMaxQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerMaxQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeIntegerMaxQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerMaxQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeIntegerMaxQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeIntegerCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerCountQs = new FunsiesSdk.collections.DudeIntegerCountQs();

// using the query method
DudeIntegerCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeIntegerCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeIntegerCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeIntegerSumQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerSumQs = new FunsiesSdk.collections.DudeIntegerSumQs();

// using the query method
DudeIntegerSumQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerSumQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeIntegerSumQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerSumQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeIntegerSumQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeStringCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeStringCountQs = new FunsiesSdk.collections.DudeStringCountQs();

// using the query method
DudeStringCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeStringCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeStringCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeStringCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeStringCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeTimeMinQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeMinQs = new FunsiesSdk.collections.DudeTimeMinQs();

// using the query method
DudeTimeMinQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeMinQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeTimeMinQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeMinQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeTimeMinQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeTimeMaxQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeMaxQs = new FunsiesSdk.collections.DudeTimeMaxQs();

// using the query method
DudeTimeMaxQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeMaxQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeTimeMaxQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeMaxQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeTimeMaxQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeTimeCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeCountQs = new FunsiesSdk.collections.DudeTimeCountQs();

// using the query method
DudeTimeCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = DudeTimeCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = DudeTimeCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####DudeFloatOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatOpTestQsEq = new FunsiesSdk.collections.DudeFloatOpTestQsEq();

// using the query method
DudeFloatOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeFloatOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatOpTestQsNe = new FunsiesSdk.collections.DudeFloatOpTestQsNe();

// using the query method
DudeFloatOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeFloatOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatOpTestQsGe = new FunsiesSdk.collections.DudeFloatOpTestQsGe();

// using the query method
DudeFloatOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeFloatOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatOpTestQsLe = new FunsiesSdk.collections.DudeFloatOpTestQsLe();

// using the query method
DudeFloatOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeFloatOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatOpTestQsGt = new FunsiesSdk.collections.DudeFloatOpTestQsGt();

// using the query method
DudeFloatOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeFloatOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatOpTestQsLt = new FunsiesSdk.collections.DudeFloatOpTestQsLt();

// using the query method
DudeFloatOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeBooleanOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeBooleanOpTestQsEq = new FunsiesSdk.collections.DudeBooleanOpTestQsEq();

// using the query method
DudeBooleanOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeBooleanOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeBooleanOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeBooleanOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeBooleanOpTestQsNe = new FunsiesSdk.collections.DudeBooleanOpTestQsNe();

// using the query method
DudeBooleanOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeBooleanOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeBooleanOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeBooleanOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeBooleanOpTestQsGe = new FunsiesSdk.collections.DudeBooleanOpTestQsGe();

// using the query method
DudeBooleanOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeBooleanOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeBooleanOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeBooleanOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeBooleanOpTestQsLe = new FunsiesSdk.collections.DudeBooleanOpTestQsLe();

// using the query method
DudeBooleanOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeBooleanOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeBooleanOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeBooleanOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeBooleanOpTestQsGt = new FunsiesSdk.collections.DudeBooleanOpTestQsGt();

// using the query method
DudeBooleanOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeBooleanOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeBooleanOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeBooleanOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeBooleanOpTestQsLt = new FunsiesSdk.collections.DudeBooleanOpTestQsLt();

// using the query method
DudeBooleanOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeBooleanOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeBooleanOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeIntegerOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerOpTestQsEq = new FunsiesSdk.collections.DudeIntegerOpTestQsEq();

// using the query method
DudeIntegerOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeIntegerOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerOpTestQsNe = new FunsiesSdk.collections.DudeIntegerOpTestQsNe();

// using the query method
DudeIntegerOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeIntegerOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerOpTestQsGe = new FunsiesSdk.collections.DudeIntegerOpTestQsGe();

// using the query method
DudeIntegerOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeIntegerOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerOpTestQsLe = new FunsiesSdk.collections.DudeIntegerOpTestQsLe();

// using the query method
DudeIntegerOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeIntegerOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerOpTestQsGt = new FunsiesSdk.collections.DudeIntegerOpTestQsGt();

// using the query method
DudeIntegerOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeIntegerOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerOpTestQsLt = new FunsiesSdk.collections.DudeIntegerOpTestQsLt();

// using the query method
DudeIntegerOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeStringOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeStringOpTestQsEq = new FunsiesSdk.collections.DudeStringOpTestQsEq();

// using the query method
DudeStringOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeStringOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeStringOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeStringOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeStringOpTestQsNe = new FunsiesSdk.collections.DudeStringOpTestQsNe();

// using the query method
DudeStringOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeStringOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeStringOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeStringOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeStringOpTestQsGe = new FunsiesSdk.collections.DudeStringOpTestQsGe();

// using the query method
DudeStringOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeStringOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeStringOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeStringOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeStringOpTestQsLe = new FunsiesSdk.collections.DudeStringOpTestQsLe();

// using the query method
DudeStringOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeStringOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeStringOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeStringOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeStringOpTestQsGt = new FunsiesSdk.collections.DudeStringOpTestQsGt();

// using the query method
DudeStringOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeStringOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeStringOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeStringOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeStringOpTestQsLt = new FunsiesSdk.collections.DudeStringOpTestQsLt();

// using the query method
DudeStringOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeStringOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeStringOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeDateOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateOpTestQsEq = new FunsiesSdk.collections.DudeDateOpTestQsEq();

// using the query method
DudeDateOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeDateOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateOpTestQsNe = new FunsiesSdk.collections.DudeDateOpTestQsNe();

// using the query method
DudeDateOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeDateOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateOpTestQsGe = new FunsiesSdk.collections.DudeDateOpTestQsGe();

// using the query method
DudeDateOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeDateOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateOpTestQsLe = new FunsiesSdk.collections.DudeDateOpTestQsLe();

// using the query method
DudeDateOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeDateOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateOpTestQsGt = new FunsiesSdk.collections.DudeDateOpTestQsGt();

// using the query method
DudeDateOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeDateOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateOpTestQsLt = new FunsiesSdk.collections.DudeDateOpTestQsLt();

// using the query method
DudeDateOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeTimeOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeOpTestQsEq = new FunsiesSdk.collections.DudeTimeOpTestQsEq();

// using the query method
DudeTimeOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeTimeOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeOpTestQsNe = new FunsiesSdk.collections.DudeTimeOpTestQsNe();

// using the query method
DudeTimeOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeTimeOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeOpTestQsGe = new FunsiesSdk.collections.DudeTimeOpTestQsGe();

// using the query method
DudeTimeOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeTimeOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeOpTestQsLe = new FunsiesSdk.collections.DudeTimeOpTestQsLe();

// using the query method
DudeTimeOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeTimeOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeOpTestQsGt = new FunsiesSdk.collections.DudeTimeOpTestQsGt();

// using the query method
DudeTimeOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeTimeOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeOpTestQsLt = new FunsiesSdk.collections.DudeTimeOpTestQsLt();

// using the query method
DudeTimeOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeFloatIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatIgnoreBlankTrueQs = new FunsiesSdk.collections.DudeFloatIgnoreBlankTrueQs();

// using the query method
DudeFloatIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_float": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_float": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_float": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeFloatIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeFloatIgnoreBlankFalseQs = new FunsiesSdk.collections.DudeFloatIgnoreBlankFalseQs();

// using the query method
DudeFloatIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_float": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeFloatIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_float": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeFloatIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_float": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeBooleanIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeBooleanIgnoreBlankTrueQs = new FunsiesSdk.collections.DudeBooleanIgnoreBlankTrueQs();

// using the query method
DudeBooleanIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeBooleanIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeBooleanIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeBooleanIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeBooleanIgnoreBlankFalseQs = new FunsiesSdk.collections.DudeBooleanIgnoreBlankFalseQs();

// using the query method
DudeBooleanIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeBooleanIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeBooleanIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeIntegerIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerIgnoreBlankTrueQs = new FunsiesSdk.collections.DudeIntegerIgnoreBlankTrueQs();

// using the query method
DudeIntegerIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeIntegerIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeIntegerIgnoreBlankFalseQs = new FunsiesSdk.collections.DudeIntegerIgnoreBlankFalseQs();

// using the query method
DudeIntegerIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeIntegerIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeIntegerIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeStringIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeStringIgnoreBlankTrueQs = new FunsiesSdk.collections.DudeStringIgnoreBlankTrueQs();

// using the query method
DudeStringIgnoreBlankTrueQs.query({
  
  "my_integer": "foo",
  
  "my_string": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeStringIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_integer": "foo",
    
    "my_string": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeStringIgnoreBlankTrueQs.query({
  
  "my_integer": "foo",
  
  "my_string": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeStringIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeStringIgnoreBlankFalseQs = new FunsiesSdk.collections.DudeStringIgnoreBlankFalseQs();

// using the query method
DudeStringIgnoreBlankFalseQs.query({
  
  "my_integer": "foo",
  
  "my_string": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeStringIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_integer": "foo",
    
    "my_string": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeStringIgnoreBlankFalseQs.query({
  
  "my_integer": "foo",
  
  "my_string": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeDateIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateIgnoreBlankTrueQs = new FunsiesSdk.collections.DudeDateIgnoreBlankTrueQs();

// using the query method
DudeDateIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_date": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_date": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_date": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeDateIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeDateIgnoreBlankFalseQs = new FunsiesSdk.collections.DudeDateIgnoreBlankFalseQs();

// using the query method
DudeDateIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_date": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeDateIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_date": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeDateIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_date": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeTimeIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeIgnoreBlankTrueQs = new FunsiesSdk.collections.DudeTimeIgnoreBlankTrueQs();

// using the query method
DudeTimeIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_time": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_time": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_time": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeTimeIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTimeIgnoreBlankFalseQs = new FunsiesSdk.collections.DudeTimeIgnoreBlankFalseQs();

// using the query method
DudeTimeIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_time": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTimeIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_time": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTimeIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_time": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeUserIdQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeUserIdQs = new FunsiesSdk.collections.DudeUserIdQs();

// using the query method
DudeUserIdQs.query({
  
  "id": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeUserIdQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "id": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeUserIdQs.query({
  
  "id": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeCustomObjectQueryScope

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeCustomObjectQueryScope = new FunsiesSdk.collections.DudeCustomObjectQueryScope();

// using the query method
DudeCustomObjectQueryScope.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeCustomObjectQueryScope.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeCustomObjectQueryScope.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeParamNameQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeParamNameQs = new FunsiesSdk.collections.DudeParamNameQs();

// using the query method
DudeParamNameQs.query({
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeParamNameQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeParamNameQs.query({
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeSingleJoinOrQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeSingleJoinOrQs = new FunsiesSdk.collections.DudeSingleJoinOrQs();

// using the query method
DudeSingleJoinOrQs.query({
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeSingleJoinOrQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeSingleJoinOrQs.query({
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeSingleJoinAndQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeSingleJoinAndQs = new FunsiesSdk.collections.DudeSingleJoinAndQs();

// using the query method
DudeSingleJoinAndQs.query({
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeSingleJoinAndQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeSingleJoinAndQs.query({
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeMultiJoinQsFirst

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeMultiJoinQsFirst = new FunsiesSdk.collections.DudeMultiJoinQsFirst();

// using the query method
DudeMultiJoinQsFirst.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeMultiJoinQsFirst.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeMultiJoinQsFirst.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeMultiJoinQsSecond

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeMultiJoinQsSecond = new FunsiesSdk.collections.DudeMultiJoinQsSecond();

// using the query method
DudeMultiJoinQsSecond.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeMultiJoinQsSecond.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeMultiJoinQsSecond.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeMultiJoinQsThird

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeMultiJoinQsThird = new FunsiesSdk.collections.DudeMultiJoinQsThird();

// using the query method
DudeMultiJoinQsThird.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeMultiJoinQsThird.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeMultiJoinQsThird.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeMultiJoinQsFourth

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeMultiJoinQsFourth = new FunsiesSdk.collections.DudeMultiJoinQsFourth();

// using the query method
DudeMultiJoinQsFourth.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeMultiJoinQsFourth.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeMultiJoinQsFourth.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeMultiJoinQsFifth

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeMultiJoinQsFifth = new FunsiesSdk.collections.DudeMultiJoinQsFifth();

// using the query method
DudeMultiJoinQsFifth.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
  "my_float": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeMultiJoinQsFifth.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
    "my_integer": "foo",
    
    "my_float": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeMultiJoinQsFifth.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
  "my_float": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####DudeTestQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var DudeTestQs = new FunsiesSdk.collections.DudeTestQs();

// using the query method
DudeTestQs.query({
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
DudeTestQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
DudeTestQs.query({
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



###Friend

####Create

This is an example of how you would create a Friend Model.

```javascript
var exampleModel = new FunsiesSdk.models.Friend();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Friend Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Friend instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Friend({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Friend objects are:

* FriendAll
* FriendExactMatch
* FriendCount
* FriendCountExactMatch
* FriendHiddenQs

#####FriendAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var FriendAll = new FunsiesSdk.collections.FriendAll();

// using the query method
FriendAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
FriendAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
FriendAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####FriendExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var FriendExactMatch = new FunsiesSdk.collections.FriendExactMatch();

// using the query method
FriendExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
FriendExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
FriendExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####FriendCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var FriendCount = new FunsiesSdk.collections.FriendCount();

// using the query method
FriendCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
FriendCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = FriendCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
FriendCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = FriendCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####FriendCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var FriendCountExactMatch = new FunsiesSdk.collections.FriendCountExactMatch();

// using the query method
FriendCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
FriendCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = FriendCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
FriendCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = FriendCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####FriendHiddenQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var FriendHiddenQs = new FunsiesSdk.collections.FriendHiddenQs();

// using the query method
FriendHiddenQs.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
FriendHiddenQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
FriendHiddenQs.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



###Goat

####Create

This is an example of how you would create a Goat Model.

```javascript
var exampleModel = new FunsiesSdk.models.Goat();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Goat Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Goat instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Goat({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Goat objects are:

* GoatAll
* GoatExactMatch
* GoatCount
* GoatCountExactMatch

#####GoatAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var GoatAll = new FunsiesSdk.collections.GoatAll();

// using the query method
GoatAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
GoatAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
GoatAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####GoatExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var GoatExactMatch = new FunsiesSdk.collections.GoatExactMatch();

// using the query method
GoatExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
GoatExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
GoatExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####GoatCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var GoatCount = new FunsiesSdk.collections.GoatCount();

// using the query method
GoatCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
GoatCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = GoatCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
GoatCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = GoatCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####GoatCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var GoatCountExactMatch = new FunsiesSdk.collections.GoatCountExactMatch();

// using the query method
GoatCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
GoatCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = GoatCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
GoatCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = GoatCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###House

####Create

This is an example of how you would create a House Model.

```javascript
var exampleModel = new FunsiesSdk.models.House();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a House Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single House instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.House({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for House objects are:

* HouseAll
* HouseExactMatch
* HouseCount
* HouseCountExactMatch

#####HouseAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var HouseAll = new FunsiesSdk.collections.HouseAll();

// using the query method
HouseAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
HouseAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
HouseAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####HouseExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var HouseExactMatch = new FunsiesSdk.collections.HouseExactMatch();

// using the query method
HouseExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
HouseExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
HouseExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####HouseCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var HouseCount = new FunsiesSdk.collections.HouseCount();

// using the query method
HouseCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
HouseCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = HouseCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
HouseCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = HouseCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####HouseCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var HouseCountExactMatch = new FunsiesSdk.collections.HouseCountExactMatch();

// using the query method
HouseCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
HouseCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = HouseCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
HouseCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = HouseCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###IncomingContact

####Create

This is an example of how you would create a IncomingContact Model.

```javascript
var exampleModel = new FunsiesSdk.models.IncomingContact();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a IncomingContact Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single IncomingContact instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.IncomingContact({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for IncomingContact objects are:

* IncomingContactAll
* IncomingContactExactMatch
* IncomingContactCount
* IncomingContactCountExactMatch

#####IncomingContactAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var IncomingContactAll = new FunsiesSdk.collections.IncomingContactAll();

// using the query method
IncomingContactAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
IncomingContactAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
IncomingContactAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####IncomingContactExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var IncomingContactExactMatch = new FunsiesSdk.collections.IncomingContactExactMatch();

// using the query method
IncomingContactExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
IncomingContactExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
IncomingContactExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####IncomingContactCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var IncomingContactCount = new FunsiesSdk.collections.IncomingContactCount();

// using the query method
IncomingContactCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
IncomingContactCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = IncomingContactCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
IncomingContactCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = IncomingContactCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####IncomingContactCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var IncomingContactCountExactMatch = new FunsiesSdk.collections.IncomingContactCountExactMatch();

// using the query method
IncomingContactCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
IncomingContactCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = IncomingContactCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
IncomingContactCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = IncomingContactCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Man

####Create

This is an example of how you would create a Man Model.

```javascript
var exampleModel = new FunsiesSdk.models.Man();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Man Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Man instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Man({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Man objects are:

* ManAll
* ManExactMatch
* ManCount
* ManCountExactMatch

#####ManAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ManAll = new FunsiesSdk.collections.ManAll();

// using the query method
ManAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ManAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ManAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####ManExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ManExactMatch = new FunsiesSdk.collections.ManExactMatch();

// using the query method
ManExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ManExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ManExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####ManCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ManCount = new FunsiesSdk.collections.ManCount();

// using the query method
ManCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ManCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = ManCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ManCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = ManCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####ManCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ManCountExactMatch = new FunsiesSdk.collections.ManCountExactMatch();

// using the query method
ManCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ManCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = ManCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ManCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = ManCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Monkey

####Create

This is an example of how you would create a Monkey Model.

```javascript
var exampleModel = new FunsiesSdk.models.Monkey();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Monkey Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Monkey instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Monkey({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Monkey objects are:

* MonkeyAll
* MonkeyExactMatch
* MonkeyCount
* MonkeyCountExactMatch

#####MonkeyAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var MonkeyAll = new FunsiesSdk.collections.MonkeyAll();

// using the query method
MonkeyAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
MonkeyAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
MonkeyAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####MonkeyExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var MonkeyExactMatch = new FunsiesSdk.collections.MonkeyExactMatch();

// using the query method
MonkeyExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
MonkeyExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
MonkeyExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####MonkeyCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var MonkeyCount = new FunsiesSdk.collections.MonkeyCount();

// using the query method
MonkeyCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
MonkeyCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = MonkeyCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
MonkeyCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = MonkeyCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####MonkeyCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var MonkeyCountExactMatch = new FunsiesSdk.collections.MonkeyCountExactMatch();

// using the query method
MonkeyCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
MonkeyCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = MonkeyCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
MonkeyCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = MonkeyCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Order

####Create

This is an example of how you would create a Order Model.

```javascript
var exampleModel = new FunsiesSdk.models.Order();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Order Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Order instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Order({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Order objects are:

* OrderAll
* OrderExactMatch
* OrderCount
* OrderCountExactMatch
* OrderOrdersInAmountRange
* OrderPaidOrdersAnd
* OrderPaidOrdersOr
* OrderCurrentUserOrders

#####OrderAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OrderAll = new FunsiesSdk.collections.OrderAll();

// using the query method
OrderAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OrderAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OrderAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####OrderExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OrderExactMatch = new FunsiesSdk.collections.OrderExactMatch();

// using the query method
OrderExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OrderExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OrderExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####OrderCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OrderCount = new FunsiesSdk.collections.OrderCount();

// using the query method
OrderCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OrderCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = OrderCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OrderCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = OrderCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####OrderCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OrderCountExactMatch = new FunsiesSdk.collections.OrderCountExactMatch();

// using the query method
OrderCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OrderCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = OrderCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OrderCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = OrderCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####OrderOrdersInAmountRange

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OrderOrdersInAmountRange = new FunsiesSdk.collections.OrderOrdersInAmountRange();

// using the query method
OrderOrdersInAmountRange.query({
  
  "start_amount": "foo",
  
  "end_amount": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OrderOrdersInAmountRange.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "start_amount": "foo",
    
    "end_amount": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OrderOrdersInAmountRange.query({
  
  "start_amount": "foo",
  
  "end_amount": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####OrderPaidOrdersAnd

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OrderPaidOrdersAnd = new FunsiesSdk.collections.OrderPaidOrdersAnd();

// using the query method
OrderPaidOrdersAnd.query({
  
  "paid": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OrderPaidOrdersAnd.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "paid": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OrderPaidOrdersAnd.query({
  
  "paid": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####OrderPaidOrdersOr

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OrderPaidOrdersOr = new FunsiesSdk.collections.OrderPaidOrdersOr();

// using the query method
OrderPaidOrdersOr.query({
  
  "paid": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OrderPaidOrdersOr.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "paid": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OrderPaidOrdersOr.query({
  
  "paid": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####OrderCurrentUserOrders

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OrderCurrentUserOrders = new FunsiesSdk.collections.OrderCurrentUserOrders();

// using the query method
OrderCurrentUserOrders.query({
  
  "id": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OrderCurrentUserOrders.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "id": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OrderCurrentUserOrders.query({
  
  "id": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



###Outage

####Create

This is an example of how you would create a Outage Model.

```javascript
var exampleModel = new FunsiesSdk.models.Outage();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Outage Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Outage instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Outage({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Outage objects are:

* OutageAll
* OutageExactMatch
* OutageCount
* OutageCountExactMatch

#####OutageAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OutageAll = new FunsiesSdk.collections.OutageAll();

// using the query method
OutageAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OutageAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OutageAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####OutageExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OutageExactMatch = new FunsiesSdk.collections.OutageExactMatch();

// using the query method
OutageExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OutageExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OutageExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####OutageCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OutageCount = new FunsiesSdk.collections.OutageCount();

// using the query method
OutageCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OutageCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = OutageCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OutageCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = OutageCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####OutageCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var OutageCountExactMatch = new FunsiesSdk.collections.OutageCountExactMatch();

// using the query method
OutageCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
OutageCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = OutageCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
OutageCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = OutageCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Pal

####Create

This is an example of how you would create a Pal Model.

```javascript
var exampleModel = new FunsiesSdk.models.Pal();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Pal Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Pal instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Pal({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Pal objects are:

* PalAll
* PalExactMatch
* PalCount
* PalCountExactMatch

#####PalAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var PalAll = new FunsiesSdk.collections.PalAll();

// using the query method
PalAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
PalAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
PalAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####PalExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var PalExactMatch = new FunsiesSdk.collections.PalExactMatch();

// using the query method
PalExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
PalExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
PalExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####PalCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var PalCount = new FunsiesSdk.collections.PalCount();

// using the query method
PalCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
PalCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = PalCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
PalCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = PalCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####PalCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var PalCountExactMatch = new FunsiesSdk.collections.PalCountExactMatch();

// using the query method
PalCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
PalCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = PalCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
PalCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = PalCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Patient

####Create

This is an example of how you would create a Patient Model.

```javascript
var exampleModel = new FunsiesSdk.models.Patient();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Patient Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Patient instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Patient({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Patient objects are:

* PatientAll
* PatientExactMatch
* PatientCount
* PatientCountExactMatch

#####PatientAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var PatientAll = new FunsiesSdk.collections.PatientAll();

// using the query method
PatientAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
PatientAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
PatientAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####PatientExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var PatientExactMatch = new FunsiesSdk.collections.PatientExactMatch();

// using the query method
PatientExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
PatientExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
PatientExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####PatientCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var PatientCount = new FunsiesSdk.collections.PatientCount();

// using the query method
PatientCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
PatientCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = PatientCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
PatientCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = PatientCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####PatientCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var PatientCountExactMatch = new FunsiesSdk.collections.PatientCountExactMatch();

// using the query method
PatientCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
PatientCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = PatientCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
PatientCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = PatientCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Product

####Create

This is an example of how you would create a Product Model.

```javascript
var exampleModel = new FunsiesSdk.models.Product();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Product Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Product instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Product({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Product objects are:

* ProductAll
* ProductExactMatch
* ProductCount
* ProductCountExactMatch
* ProductSale
* ProductProductsByCategory

#####ProductAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ProductAll = new FunsiesSdk.collections.ProductAll();

// using the query method
ProductAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ProductAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ProductAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####ProductExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ProductExactMatch = new FunsiesSdk.collections.ProductExactMatch();

// using the query method
ProductExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ProductExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ProductExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####ProductCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ProductCount = new FunsiesSdk.collections.ProductCount();

// using the query method
ProductCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ProductCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = ProductCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ProductCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = ProductCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####ProductCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ProductCountExactMatch = new FunsiesSdk.collections.ProductCountExactMatch();

// using the query method
ProductCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ProductCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = ProductCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ProductCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = ProductCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####ProductSale

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ProductSale = new FunsiesSdk.collections.ProductSale();

// using the query method
ProductSale.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ProductSale.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ProductSale.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####ProductProductsByCategory

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var ProductProductsByCategory = new FunsiesSdk.collections.ProductProductsByCategory();

// using the query method
ProductProductsByCategory.query({
  
  "name": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
ProductProductsByCategory.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "name": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
ProductProductsByCategory.query({
  
  "name": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



###RelationalDude

####Create

This is an example of how you would create a RelationalDude Model.

```javascript
var exampleModel = new FunsiesSdk.models.RelationalDude();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a RelationalDude Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single RelationalDude instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.RelationalDude({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for RelationalDude objects are:

* RelationalDudeAll
* RelationalDudeExactMatch
* RelationalDudeCount
* RelationalDudeCountExactMatch
* RelationalDudeBooleanAssignableQs
* RelationalDudeDateAssignableQs
* RelationalDudeTimeAssignableQs
* RelationalDudeFloatAssignableQs
* RelationalDudeIntegerAssignableQs
* RelationalDudeStringAssignableQs
* RelationalDudeBooleanDefaultValueQs
* RelationalDudeBooleanCountQs
* RelationalDudeDateMinQs
* RelationalDudeDateMaxQs
* RelationalDudeDateCountQs
* RelationalDudeFloatAvgQs
* RelationalDudeFloatMinQs
* RelationalDudeFloatMaxQs
* RelationalDudeFloatCountQs
* RelationalDudeFloatSumQs
* RelationalDudeIntegerAvgQs
* RelationalDudeIntegerMinQs
* RelationalDudeIntegerMaxQs
* RelationalDudeIntegerCountQs
* RelationalDudeIntegerSumQs
* RelationalDudeStringCountQs
* RelationalDudeTimeMinQs
* RelationalDudeTimeMaxQs
* RelationalDudeTimeCountQs
* RelationalDudeFloatOpTestQsEq
* RelationalDudeFloatOpTestQsNe
* RelationalDudeFloatOpTestQsGe
* RelationalDudeFloatOpTestQsLe
* RelationalDudeFloatOpTestQsGt
* RelationalDudeFloatOpTestQsLt
* RelationalDudeBooleanOpTestQsEq
* RelationalDudeBooleanOpTestQsNe
* RelationalDudeBooleanOpTestQsGe
* RelationalDudeBooleanOpTestQsLe
* RelationalDudeBooleanOpTestQsGt
* RelationalDudeBooleanOpTestQsLt
* RelationalDudeIntegerOpTestQsEq
* RelationalDudeIntegerOpTestQsNe
* RelationalDudeIntegerOpTestQsGe
* RelationalDudeIntegerOpTestQsLe
* RelationalDudeIntegerOpTestQsGt
* RelationalDudeIntegerOpTestQsLt
* RelationalDudeStringOpTestQsEq
* RelationalDudeStringOpTestQsNe
* RelationalDudeStringOpTestQsGe
* RelationalDudeStringOpTestQsLe
* RelationalDudeStringOpTestQsGt
* RelationalDudeStringOpTestQsLt
* RelationalDudeDateOpTestQsEq
* RelationalDudeDateOpTestQsNe
* RelationalDudeDateOpTestQsGe
* RelationalDudeDateOpTestQsLe
* RelationalDudeDateOpTestQsGt
* RelationalDudeDateOpTestQsLt
* RelationalDudeTimeOpTestQsEq
* RelationalDudeTimeOpTestQsNe
* RelationalDudeTimeOpTestQsGe
* RelationalDudeTimeOpTestQsLe
* RelationalDudeTimeOpTestQsGt
* RelationalDudeTimeOpTestQsLt
* RelationalDudeFloatIgnoreBlankTrueQs
* RelationalDudeFloatIgnoreBlankFalseQs
* RelationalDudeBooleanIgnoreBlankTrueQs
* RelationalDudeBooleanIgnoreBlankFalseQs
* RelationalDudeIntegerIgnoreBlankTrueQs
* RelationalDudeIntegerIgnoreBlankFalseQs
* RelationalDudeStringIgnoreBlankTrueQs
* RelationalDudeStringIgnoreBlankFalseQs
* RelationalDudeDateIgnoreBlankTrueQs
* RelationalDudeDateIgnoreBlankFalseQs
* RelationalDudeTimeIgnoreBlankTrueQs
* RelationalDudeTimeIgnoreBlankFalseQs
* RelationalDudeUserIdQs
* RelationalDudeCustomObjectQueryScope
* RelationalDudeParamNameQs
* RelationalDudeSingleJoinOrQs
* RelationalDudeSingleJoinAndQs
* RelationalDudeMultiJoinQsFirst
* RelationalDudeMultiJoinQsSecond
* RelationalDudeMultiJoinQsThird
* RelationalDudeMultiJoinQsFourth
* RelationalDudeMultiJoinQsFifth
* RelationalDudeTestQs

#####RelationalDudeAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeAll = new FunsiesSdk.collections.RelationalDudeAll();

// using the query method
RelationalDudeAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeExactMatch = new FunsiesSdk.collections.RelationalDudeExactMatch();

// using the query method
RelationalDudeExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeCount = new FunsiesSdk.collections.RelationalDudeCount();

// using the query method
RelationalDudeCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeCountExactMatch = new FunsiesSdk.collections.RelationalDudeCountExactMatch();

// using the query method
RelationalDudeCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeBooleanAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeBooleanAssignableQs = new FunsiesSdk.collections.RelationalDudeBooleanAssignableQs();

// using the query method
RelationalDudeBooleanAssignableQs.query({
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeBooleanAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeBooleanAssignableQs.query({
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeDateAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateAssignableQs = new FunsiesSdk.collections.RelationalDudeDateAssignableQs();

// using the query method
RelationalDudeDateAssignableQs.query({
  
  "my_date": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_date": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateAssignableQs.query({
  
  "my_date": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeTimeAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeAssignableQs = new FunsiesSdk.collections.RelationalDudeTimeAssignableQs();

// using the query method
RelationalDudeTimeAssignableQs.query({
  
  "my_time": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_time": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeAssignableQs.query({
  
  "my_time": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeFloatAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatAssignableQs = new FunsiesSdk.collections.RelationalDudeFloatAssignableQs();

// using the query method
RelationalDudeFloatAssignableQs.query({
  
  "my_float": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_float": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatAssignableQs.query({
  
  "my_float": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeIntegerAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerAssignableQs = new FunsiesSdk.collections.RelationalDudeIntegerAssignableQs();

// using the query method
RelationalDudeIntegerAssignableQs.query({
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerAssignableQs.query({
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeStringAssignableQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeStringAssignableQs = new FunsiesSdk.collections.RelationalDudeStringAssignableQs();

// using the query method
RelationalDudeStringAssignableQs.query({
  
  "my_string": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeStringAssignableQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeStringAssignableQs.query({
  
  "my_string": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeBooleanDefaultValueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeBooleanDefaultValueQs = new FunsiesSdk.collections.RelationalDudeBooleanDefaultValueQs();

// using the query method
RelationalDudeBooleanDefaultValueQs.query({
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeBooleanDefaultValueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeBooleanDefaultValueQs.query({
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeBooleanCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeBooleanCountQs = new FunsiesSdk.collections.RelationalDudeBooleanCountQs();

// using the query method
RelationalDudeBooleanCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeBooleanCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeBooleanCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeBooleanCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeBooleanCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeDateMinQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateMinQs = new FunsiesSdk.collections.RelationalDudeDateMinQs();

// using the query method
RelationalDudeDateMinQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateMinQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeDateMinQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateMinQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeDateMinQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeDateMaxQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateMaxQs = new FunsiesSdk.collections.RelationalDudeDateMaxQs();

// using the query method
RelationalDudeDateMaxQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateMaxQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeDateMaxQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateMaxQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeDateMaxQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeDateCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateCountQs = new FunsiesSdk.collections.RelationalDudeDateCountQs();

// using the query method
RelationalDudeDateCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeDateCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeDateCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeFloatAvgQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatAvgQs = new FunsiesSdk.collections.RelationalDudeFloatAvgQs();

// using the query method
RelationalDudeFloatAvgQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatAvgQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeFloatAvgQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatAvgQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeFloatAvgQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeFloatMinQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatMinQs = new FunsiesSdk.collections.RelationalDudeFloatMinQs();

// using the query method
RelationalDudeFloatMinQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatMinQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeFloatMinQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatMinQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeFloatMinQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeFloatMaxQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatMaxQs = new FunsiesSdk.collections.RelationalDudeFloatMaxQs();

// using the query method
RelationalDudeFloatMaxQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatMaxQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeFloatMaxQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatMaxQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeFloatMaxQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeFloatCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatCountQs = new FunsiesSdk.collections.RelationalDudeFloatCountQs();

// using the query method
RelationalDudeFloatCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeFloatCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeFloatCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeFloatSumQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatSumQs = new FunsiesSdk.collections.RelationalDudeFloatSumQs();

// using the query method
RelationalDudeFloatSumQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatSumQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeFloatSumQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatSumQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeFloatSumQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeIntegerAvgQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerAvgQs = new FunsiesSdk.collections.RelationalDudeIntegerAvgQs();

// using the query method
RelationalDudeIntegerAvgQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerAvgQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeIntegerAvgQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerAvgQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeIntegerAvgQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeIntegerMinQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerMinQs = new FunsiesSdk.collections.RelationalDudeIntegerMinQs();

// using the query method
RelationalDudeIntegerMinQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerMinQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeIntegerMinQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerMinQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeIntegerMinQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeIntegerMaxQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerMaxQs = new FunsiesSdk.collections.RelationalDudeIntegerMaxQs();

// using the query method
RelationalDudeIntegerMaxQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerMaxQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeIntegerMaxQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerMaxQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeIntegerMaxQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeIntegerCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerCountQs = new FunsiesSdk.collections.RelationalDudeIntegerCountQs();

// using the query method
RelationalDudeIntegerCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeIntegerCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeIntegerCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeIntegerSumQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerSumQs = new FunsiesSdk.collections.RelationalDudeIntegerSumQs();

// using the query method
RelationalDudeIntegerSumQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerSumQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeIntegerSumQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerSumQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeIntegerSumQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeStringCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeStringCountQs = new FunsiesSdk.collections.RelationalDudeStringCountQs();

// using the query method
RelationalDudeStringCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeStringCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeStringCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeStringCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeStringCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeTimeMinQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeMinQs = new FunsiesSdk.collections.RelationalDudeTimeMinQs();

// using the query method
RelationalDudeTimeMinQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeMinQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeTimeMinQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeMinQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeTimeMinQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeTimeMaxQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeMaxQs = new FunsiesSdk.collections.RelationalDudeTimeMaxQs();

// using the query method
RelationalDudeTimeMaxQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeMaxQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeTimeMaxQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeMaxQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeTimeMaxQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeTimeCountQs

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeCountQs = new FunsiesSdk.collections.RelationalDudeTimeCountQs();

// using the query method
RelationalDudeTimeCountQs.query({
  
  "": "foo",
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeCountQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RelationalDudeTimeCountQs.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeCountQs.query({
  
  "": "foo",
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RelationalDudeTimeCountQs.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RelationalDudeFloatOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatOpTestQsEq = new FunsiesSdk.collections.RelationalDudeFloatOpTestQsEq();

// using the query method
RelationalDudeFloatOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeFloatOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatOpTestQsNe = new FunsiesSdk.collections.RelationalDudeFloatOpTestQsNe();

// using the query method
RelationalDudeFloatOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeFloatOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatOpTestQsGe = new FunsiesSdk.collections.RelationalDudeFloatOpTestQsGe();

// using the query method
RelationalDudeFloatOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeFloatOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatOpTestQsLe = new FunsiesSdk.collections.RelationalDudeFloatOpTestQsLe();

// using the query method
RelationalDudeFloatOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeFloatOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatOpTestQsGt = new FunsiesSdk.collections.RelationalDudeFloatOpTestQsGt();

// using the query method
RelationalDudeFloatOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeFloatOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatOpTestQsLt = new FunsiesSdk.collections.RelationalDudeFloatOpTestQsLt();

// using the query method
RelationalDudeFloatOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeBooleanOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeBooleanOpTestQsEq = new FunsiesSdk.collections.RelationalDudeBooleanOpTestQsEq();

// using the query method
RelationalDudeBooleanOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeBooleanOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeBooleanOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeBooleanOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeBooleanOpTestQsNe = new FunsiesSdk.collections.RelationalDudeBooleanOpTestQsNe();

// using the query method
RelationalDudeBooleanOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeBooleanOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeBooleanOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeBooleanOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeBooleanOpTestQsGe = new FunsiesSdk.collections.RelationalDudeBooleanOpTestQsGe();

// using the query method
RelationalDudeBooleanOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeBooleanOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeBooleanOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeBooleanOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeBooleanOpTestQsLe = new FunsiesSdk.collections.RelationalDudeBooleanOpTestQsLe();

// using the query method
RelationalDudeBooleanOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeBooleanOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeBooleanOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeBooleanOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeBooleanOpTestQsGt = new FunsiesSdk.collections.RelationalDudeBooleanOpTestQsGt();

// using the query method
RelationalDudeBooleanOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeBooleanOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeBooleanOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeBooleanOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeBooleanOpTestQsLt = new FunsiesSdk.collections.RelationalDudeBooleanOpTestQsLt();

// using the query method
RelationalDudeBooleanOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeBooleanOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeBooleanOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeIntegerOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerOpTestQsEq = new FunsiesSdk.collections.RelationalDudeIntegerOpTestQsEq();

// using the query method
RelationalDudeIntegerOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeIntegerOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerOpTestQsNe = new FunsiesSdk.collections.RelationalDudeIntegerOpTestQsNe();

// using the query method
RelationalDudeIntegerOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeIntegerOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerOpTestQsGe = new FunsiesSdk.collections.RelationalDudeIntegerOpTestQsGe();

// using the query method
RelationalDudeIntegerOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeIntegerOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerOpTestQsLe = new FunsiesSdk.collections.RelationalDudeIntegerOpTestQsLe();

// using the query method
RelationalDudeIntegerOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeIntegerOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerOpTestQsGt = new FunsiesSdk.collections.RelationalDudeIntegerOpTestQsGt();

// using the query method
RelationalDudeIntegerOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeIntegerOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerOpTestQsLt = new FunsiesSdk.collections.RelationalDudeIntegerOpTestQsLt();

// using the query method
RelationalDudeIntegerOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeStringOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeStringOpTestQsEq = new FunsiesSdk.collections.RelationalDudeStringOpTestQsEq();

// using the query method
RelationalDudeStringOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeStringOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeStringOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeStringOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeStringOpTestQsNe = new FunsiesSdk.collections.RelationalDudeStringOpTestQsNe();

// using the query method
RelationalDudeStringOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeStringOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeStringOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeStringOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeStringOpTestQsGe = new FunsiesSdk.collections.RelationalDudeStringOpTestQsGe();

// using the query method
RelationalDudeStringOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeStringOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeStringOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeStringOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeStringOpTestQsLe = new FunsiesSdk.collections.RelationalDudeStringOpTestQsLe();

// using the query method
RelationalDudeStringOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeStringOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeStringOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeStringOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeStringOpTestQsGt = new FunsiesSdk.collections.RelationalDudeStringOpTestQsGt();

// using the query method
RelationalDudeStringOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeStringOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeStringOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeStringOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeStringOpTestQsLt = new FunsiesSdk.collections.RelationalDudeStringOpTestQsLt();

// using the query method
RelationalDudeStringOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeStringOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeStringOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeDateOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateOpTestQsEq = new FunsiesSdk.collections.RelationalDudeDateOpTestQsEq();

// using the query method
RelationalDudeDateOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeDateOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateOpTestQsNe = new FunsiesSdk.collections.RelationalDudeDateOpTestQsNe();

// using the query method
RelationalDudeDateOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeDateOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateOpTestQsGe = new FunsiesSdk.collections.RelationalDudeDateOpTestQsGe();

// using the query method
RelationalDudeDateOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeDateOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateOpTestQsLe = new FunsiesSdk.collections.RelationalDudeDateOpTestQsLe();

// using the query method
RelationalDudeDateOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeDateOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateOpTestQsGt = new FunsiesSdk.collections.RelationalDudeDateOpTestQsGt();

// using the query method
RelationalDudeDateOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeDateOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateOpTestQsLt = new FunsiesSdk.collections.RelationalDudeDateOpTestQsLt();

// using the query method
RelationalDudeDateOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeTimeOpTestQsEq

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeOpTestQsEq = new FunsiesSdk.collections.RelationalDudeTimeOpTestQsEq();

// using the query method
RelationalDudeTimeOpTestQsEq.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeOpTestQsEq.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeOpTestQsEq.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeTimeOpTestQsNe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeOpTestQsNe = new FunsiesSdk.collections.RelationalDudeTimeOpTestQsNe();

// using the query method
RelationalDudeTimeOpTestQsNe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeOpTestQsNe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeOpTestQsNe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeTimeOpTestQsGe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeOpTestQsGe = new FunsiesSdk.collections.RelationalDudeTimeOpTestQsGe();

// using the query method
RelationalDudeTimeOpTestQsGe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeOpTestQsGe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeOpTestQsGe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeTimeOpTestQsLe

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeOpTestQsLe = new FunsiesSdk.collections.RelationalDudeTimeOpTestQsLe();

// using the query method
RelationalDudeTimeOpTestQsLe.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeOpTestQsLe.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeOpTestQsLe.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeTimeOpTestQsGt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeOpTestQsGt = new FunsiesSdk.collections.RelationalDudeTimeOpTestQsGt();

// using the query method
RelationalDudeTimeOpTestQsGt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeOpTestQsGt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeOpTestQsGt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeTimeOpTestQsLt

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeOpTestQsLt = new FunsiesSdk.collections.RelationalDudeTimeOpTestQsLt();

// using the query method
RelationalDudeTimeOpTestQsLt.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeOpTestQsLt.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeOpTestQsLt.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeFloatIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatIgnoreBlankTrueQs = new FunsiesSdk.collections.RelationalDudeFloatIgnoreBlankTrueQs();

// using the query method
RelationalDudeFloatIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_float": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_float": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_float": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeFloatIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeFloatIgnoreBlankFalseQs = new FunsiesSdk.collections.RelationalDudeFloatIgnoreBlankFalseQs();

// using the query method
RelationalDudeFloatIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_float": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeFloatIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_float": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeFloatIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_float": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeBooleanIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeBooleanIgnoreBlankTrueQs = new FunsiesSdk.collections.RelationalDudeBooleanIgnoreBlankTrueQs();

// using the query method
RelationalDudeBooleanIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeBooleanIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeBooleanIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeBooleanIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeBooleanIgnoreBlankFalseQs = new FunsiesSdk.collections.RelationalDudeBooleanIgnoreBlankFalseQs();

// using the query method
RelationalDudeBooleanIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeBooleanIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeBooleanIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeIntegerIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerIgnoreBlankTrueQs = new FunsiesSdk.collections.RelationalDudeIntegerIgnoreBlankTrueQs();

// using the query method
RelationalDudeIntegerIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeIntegerIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeIntegerIgnoreBlankFalseQs = new FunsiesSdk.collections.RelationalDudeIntegerIgnoreBlankFalseQs();

// using the query method
RelationalDudeIntegerIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeIntegerIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeIntegerIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeStringIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeStringIgnoreBlankTrueQs = new FunsiesSdk.collections.RelationalDudeStringIgnoreBlankTrueQs();

// using the query method
RelationalDudeStringIgnoreBlankTrueQs.query({
  
  "my_integer": "foo",
  
  "my_string": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeStringIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_integer": "foo",
    
    "my_string": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeStringIgnoreBlankTrueQs.query({
  
  "my_integer": "foo",
  
  "my_string": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeStringIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeStringIgnoreBlankFalseQs = new FunsiesSdk.collections.RelationalDudeStringIgnoreBlankFalseQs();

// using the query method
RelationalDudeStringIgnoreBlankFalseQs.query({
  
  "my_integer": "foo",
  
  "my_string": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeStringIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_integer": "foo",
    
    "my_string": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeStringIgnoreBlankFalseQs.query({
  
  "my_integer": "foo",
  
  "my_string": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeDateIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateIgnoreBlankTrueQs = new FunsiesSdk.collections.RelationalDudeDateIgnoreBlankTrueQs();

// using the query method
RelationalDudeDateIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_date": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_date": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_date": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeDateIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeDateIgnoreBlankFalseQs = new FunsiesSdk.collections.RelationalDudeDateIgnoreBlankFalseQs();

// using the query method
RelationalDudeDateIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_date": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeDateIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_date": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeDateIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_date": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeTimeIgnoreBlankTrueQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeIgnoreBlankTrueQs = new FunsiesSdk.collections.RelationalDudeTimeIgnoreBlankTrueQs();

// using the query method
RelationalDudeTimeIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_time": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeIgnoreBlankTrueQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_time": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeIgnoreBlankTrueQs.query({
  
  "my_string": "foo",
  
  "my_time": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeTimeIgnoreBlankFalseQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTimeIgnoreBlankFalseQs = new FunsiesSdk.collections.RelationalDudeTimeIgnoreBlankFalseQs();

// using the query method
RelationalDudeTimeIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_time": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTimeIgnoreBlankFalseQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_string": "foo",
    
    "my_time": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTimeIgnoreBlankFalseQs.query({
  
  "my_string": "foo",
  
  "my_time": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeUserIdQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeUserIdQs = new FunsiesSdk.collections.RelationalDudeUserIdQs();

// using the query method
RelationalDudeUserIdQs.query({
  
  "id": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeUserIdQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "id": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeUserIdQs.query({
  
  "id": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeCustomObjectQueryScope

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeCustomObjectQueryScope = new FunsiesSdk.collections.RelationalDudeCustomObjectQueryScope();

// using the query method
RelationalDudeCustomObjectQueryScope.query({
  
  "": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeCustomObjectQueryScope.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeCustomObjectQueryScope.query({
  
  "": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeParamNameQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeParamNameQs = new FunsiesSdk.collections.RelationalDudeParamNameQs();

// using the query method
RelationalDudeParamNameQs.query({
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeParamNameQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeParamNameQs.query({
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeSingleJoinOrQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeSingleJoinOrQs = new FunsiesSdk.collections.RelationalDudeSingleJoinOrQs();

// using the query method
RelationalDudeSingleJoinOrQs.query({
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeSingleJoinOrQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeSingleJoinOrQs.query({
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeSingleJoinAndQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeSingleJoinAndQs = new FunsiesSdk.collections.RelationalDudeSingleJoinAndQs();

// using the query method
RelationalDudeSingleJoinAndQs.query({
  
  "my_boolean": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeSingleJoinAndQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeSingleJoinAndQs.query({
  
  "my_boolean": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeMultiJoinQsFirst

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeMultiJoinQsFirst = new FunsiesSdk.collections.RelationalDudeMultiJoinQsFirst();

// using the query method
RelationalDudeMultiJoinQsFirst.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeMultiJoinQsFirst.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeMultiJoinQsFirst.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeMultiJoinQsSecond

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeMultiJoinQsSecond = new FunsiesSdk.collections.RelationalDudeMultiJoinQsSecond();

// using the query method
RelationalDudeMultiJoinQsSecond.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeMultiJoinQsSecond.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeMultiJoinQsSecond.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeMultiJoinQsThird

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeMultiJoinQsThird = new FunsiesSdk.collections.RelationalDudeMultiJoinQsThird();

// using the query method
RelationalDudeMultiJoinQsThird.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeMultiJoinQsThird.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeMultiJoinQsThird.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeMultiJoinQsFourth

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeMultiJoinQsFourth = new FunsiesSdk.collections.RelationalDudeMultiJoinQsFourth();

// using the query method
RelationalDudeMultiJoinQsFourth.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeMultiJoinQsFourth.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeMultiJoinQsFourth.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeMultiJoinQsFifth

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeMultiJoinQsFifth = new FunsiesSdk.collections.RelationalDudeMultiJoinQsFifth();

// using the query method
RelationalDudeMultiJoinQsFifth.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
  "my_float": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeMultiJoinQsFifth.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_boolean": "foo",
    
    "my_integer": "foo",
    
    "my_float": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeMultiJoinQsFifth.query({
  
  "my_boolean": "foo",
  
  "my_integer": "foo",
  
  "my_float": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RelationalDudeTestQs

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RelationalDudeTestQs = new FunsiesSdk.collections.RelationalDudeTestQs();

// using the query method
RelationalDudeTestQs.query({
  
  "my_integer": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RelationalDudeTestQs.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "my_integer": "foo",
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RelationalDudeTestQs.query({
  
  "my_integer": "foo",
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



###Restaurant

####Create

This is an example of how you would create a Restaurant Model.

```javascript
var exampleModel = new FunsiesSdk.models.Restaurant();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Restaurant Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Restaurant instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Restaurant({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Restaurant objects are:

* RestaurantAll
* RestaurantExactMatch
* RestaurantCount
* RestaurantCountExactMatch

#####RestaurantAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RestaurantAll = new FunsiesSdk.collections.RestaurantAll();

// using the query method
RestaurantAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RestaurantAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RestaurantAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RestaurantExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RestaurantExactMatch = new FunsiesSdk.collections.RestaurantExactMatch();

// using the query method
RestaurantExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RestaurantExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RestaurantExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RestaurantCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RestaurantCount = new FunsiesSdk.collections.RestaurantCount();

// using the query method
RestaurantCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RestaurantCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RestaurantCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RestaurantCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RestaurantCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RestaurantCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RestaurantCountExactMatch = new FunsiesSdk.collections.RestaurantCountExactMatch();

// using the query method
RestaurantCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RestaurantCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RestaurantCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RestaurantCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RestaurantCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Robot

####Create

This is an example of how you would create a Robot Model.

```javascript
var exampleModel = new FunsiesSdk.models.Robot();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Robot Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Robot instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Robot({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Robot objects are:

* RobotAll
* RobotExactMatch
* RobotCount
* RobotCountExactMatch

#####RobotAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RobotAll = new FunsiesSdk.collections.RobotAll();

// using the query method
RobotAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RobotAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RobotAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RobotExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RobotExactMatch = new FunsiesSdk.collections.RobotExactMatch();

// using the query method
RobotExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RobotExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RobotExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####RobotCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RobotCount = new FunsiesSdk.collections.RobotCount();

// using the query method
RobotCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RobotCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RobotCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RobotCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RobotCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####RobotCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var RobotCountExactMatch = new FunsiesSdk.collections.RobotCountExactMatch();

// using the query method
RobotCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
RobotCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = RobotCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
RobotCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = RobotCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###SalesReport

####Create

This is an example of how you would create a SalesReport Model.

```javascript
var exampleModel = new FunsiesSdk.models.SalesReport();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a SalesReport Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single SalesReport instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.SalesReport({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for SalesReport objects are:

* SalesReportAll
* SalesReportExactMatch
* SalesReportCount
* SalesReportCountExactMatch

#####SalesReportAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesReportAll = new FunsiesSdk.collections.SalesReportAll();

// using the query method
SalesReportAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesReportAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesReportAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####SalesReportExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesReportExactMatch = new FunsiesSdk.collections.SalesReportExactMatch();

// using the query method
SalesReportExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesReportExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesReportExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####SalesReportCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesReportCount = new FunsiesSdk.collections.SalesReportCount();

// using the query method
SalesReportCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesReportCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = SalesReportCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesReportCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = SalesReportCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####SalesReportCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesReportCountExactMatch = new FunsiesSdk.collections.SalesReportCountExactMatch();

// using the query method
SalesReportCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesReportCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = SalesReportCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesReportCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = SalesReportCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###SalesforceAccount

####Create

This is an example of how you would create a SalesforceAccount Model.

```javascript
var exampleModel = new FunsiesSdk.models.SalesforceAccount();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a SalesforceAccount Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single SalesforceAccount instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.SalesforceAccount({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for SalesforceAccount objects are:

* SalesforceAccountAll
* SalesforceAccountExactMatch
* SalesforceAccountCount
* SalesforceAccountCountExactMatch

#####SalesforceAccountAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesforceAccountAll = new FunsiesSdk.collections.SalesforceAccountAll();

// using the query method
SalesforceAccountAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesforceAccountAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesforceAccountAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####SalesforceAccountExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesforceAccountExactMatch = new FunsiesSdk.collections.SalesforceAccountExactMatch();

// using the query method
SalesforceAccountExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesforceAccountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesforceAccountExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####SalesforceAccountCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesforceAccountCount = new FunsiesSdk.collections.SalesforceAccountCount();

// using the query method
SalesforceAccountCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesforceAccountCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = SalesforceAccountCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesforceAccountCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = SalesforceAccountCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####SalesforceAccountCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesforceAccountCountExactMatch = new FunsiesSdk.collections.SalesforceAccountCountExactMatch();

// using the query method
SalesforceAccountCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesforceAccountCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = SalesforceAccountCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesforceAccountCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = SalesforceAccountCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###SalesforceContact

####Create

This is an example of how you would create a SalesforceContact Model.

```javascript
var exampleModel = new FunsiesSdk.models.SalesforceContact();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a SalesforceContact Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single SalesforceContact instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.SalesforceContact({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for SalesforceContact objects are:

* SalesforceContactAll
* SalesforceContactExactMatch
* SalesforceContactCount
* SalesforceContactCountExactMatch

#####SalesforceContactAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesforceContactAll = new FunsiesSdk.collections.SalesforceContactAll();

// using the query method
SalesforceContactAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesforceContactAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesforceContactAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####SalesforceContactExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesforceContactExactMatch = new FunsiesSdk.collections.SalesforceContactExactMatch();

// using the query method
SalesforceContactExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesforceContactExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesforceContactExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####SalesforceContactCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesforceContactCount = new FunsiesSdk.collections.SalesforceContactCount();

// using the query method
SalesforceContactCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesforceContactCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = SalesforceContactCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesforceContactCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = SalesforceContactCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####SalesforceContactCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SalesforceContactCountExactMatch = new FunsiesSdk.collections.SalesforceContactCountExactMatch();

// using the query method
SalesforceContactCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SalesforceContactCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = SalesforceContactCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SalesforceContactCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = SalesforceContactCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Store

####Create

This is an example of how you would create a Store Model.

```javascript
var exampleModel = new FunsiesSdk.models.Store();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Store Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Store instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Store({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Store objects are:

* StoreAll
* StoreExactMatch
* StoreCount
* StoreCountExactMatch

#####StoreAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var StoreAll = new FunsiesSdk.collections.StoreAll();

// using the query method
StoreAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
StoreAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
StoreAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####StoreExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var StoreExactMatch = new FunsiesSdk.collections.StoreExactMatch();

// using the query method
StoreExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
StoreExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
StoreExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####StoreCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var StoreCount = new FunsiesSdk.collections.StoreCount();

// using the query method
StoreCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
StoreCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = StoreCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
StoreCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = StoreCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####StoreCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var StoreCountExactMatch = new FunsiesSdk.collections.StoreCountExactMatch();

// using the query method
StoreCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
StoreCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = StoreCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
StoreCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = StoreCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Subscriber

####Create

This is an example of how you would create a Subscriber Model.

```javascript
var exampleModel = new FunsiesSdk.models.Subscriber();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Subscriber Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Subscriber instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Subscriber({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Subscriber objects are:

* SubscriberAll
* SubscriberExactMatch
* SubscriberCount
* SubscriberCountExactMatch

#####SubscriberAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SubscriberAll = new FunsiesSdk.collections.SubscriberAll();

// using the query method
SubscriberAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SubscriberAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SubscriberAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####SubscriberExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SubscriberExactMatch = new FunsiesSdk.collections.SubscriberExactMatch();

// using the query method
SubscriberExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SubscriberExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SubscriberExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####SubscriberCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SubscriberCount = new FunsiesSdk.collections.SubscriberCount();

// using the query method
SubscriberCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SubscriberCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = SubscriberCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SubscriberCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = SubscriberCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####SubscriberCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var SubscriberCountExactMatch = new FunsiesSdk.collections.SubscriberCountExactMatch();

// using the query method
SubscriberCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
SubscriberCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = SubscriberCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
SubscriberCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = SubscriberCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###User

####Create

This is an example of how you would create a User Model.

```javascript
var exampleModel = new FunsiesSdk.models.User();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a User Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single User instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.User({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for User objects are:

* UserAll
* UserExactMatch
* UserCount
* UserCountExactMatch

#####UserAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var UserAll = new FunsiesSdk.collections.UserAll();

// using the query method
UserAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
UserAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
UserAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####UserExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var UserExactMatch = new FunsiesSdk.collections.UserExactMatch();

// using the query method
UserExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
UserExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
UserExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####UserCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var UserCount = new FunsiesSdk.collections.UserCount();

// using the query method
UserCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
UserCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = UserCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
UserCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = UserCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####UserCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var UserCountExactMatch = new FunsiesSdk.collections.UserCountExactMatch();

// using the query method
UserCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
UserCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = UserCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
UserCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = UserCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


###Wizard

####Create

This is an example of how you would create a Wizard Model.

```javascript
var exampleModel = new FunsiesSdk.models.Wizard();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a Wizard Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single Wizard instance by its primary key.

```javascript
var singleInstance = new FunsiesSdk.models.Wizard({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for Wizard objects are:

* WizardAll
* WizardExactMatch
* WizardCount
* WizardCountExactMatch

#####WizardAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var WizardAll = new FunsiesSdk.collections.WizardAll();

// using the query method
WizardAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
WizardAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
WizardAll.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####WizardExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var WizardExactMatch = new FunsiesSdk.collections.WizardExactMatch();

// using the query method
WizardExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
WizardExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
WizardExactMatch.query({
  
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.



#####WizardCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var WizardCount = new FunsiesSdk.collections.WizardCount();

// using the query method
WizardCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
WizardCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = WizardCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
WizardCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = WizardCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


#####WizardCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var WizardCountExactMatch = new FunsiesSdk.collections.WizardCountExactMatch();

// using the query method
WizardCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
WizardCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = WizardCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
WizardCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = WizardCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


