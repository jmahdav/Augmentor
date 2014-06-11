Augmentor
=========
;; writing a test for Augmentor service

	;; testing engine Augment
	when (event.key-attribute == augment.key-attribute)
		if (event.attributes.name == augment.attributes.name)     ;;to override and attribute 
			event.attributes.value = augment.attributes.value
			(conj event augment)

     ;; testing notification Augment
     when (event.key-attribute == augment.key-attribute)
     	if (pattern match)
     		(conj augment notification)

     ;;augment API service 
     when (key-Attribute = empty || content-type == application/json )
        println ("an error has been ocurred")
