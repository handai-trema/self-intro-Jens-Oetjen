I modified the "start-function" of the example-program according to the following code snippet:

```Ruby

   def start(_args)
   
    logger.info "#{self.class.name} started"
    
  end

```

Self references to the class which is currently been used and class.name references to the name of the class. With this change, the message "HelloTrema started" is displayed as requested 
without using the "forbidden" code snippet.