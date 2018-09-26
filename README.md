### RailsAdmin rails_admin
---

https://github.com/sferik/rails_admin

```sh
gem 'rails_admin', '~> 1.3'
bundle install
rails g rails_admin:install
rails s
```

config/initializers/rails_admin.rb
```ruby
class Ball < ActiveRecord::Base
  validates :name, presence: true
  belongs_to :player
  
  rails_admin do
    configure :player do
      label 'Owner of this ball: '
    end
  end
end

```
https://github.com/sferik/rails_admin/wiki

https://github.com/bbenezech/dummy_app
http://rails-admin-tb.herokuapp.com/

