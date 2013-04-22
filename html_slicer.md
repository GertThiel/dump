# html_slicer

[Split HTML text in 2 paragraphs](http://stackoverflow.com/questions/2618932/split-html-text-in-2-paragraphs) using [addagger/html_slicer](https://github.com/addagger/html_slicer)

## Gemfile

    gem 'html_slicer', :require => nil

## Usage

    complement = Complement.find(2615160)
    content = complement.value

    sliced = HtmlSlicer::Interface.new(content, :to_s, { :slice => { :complete => /\s+|\z/, :maximum => content.dehtml.length/10 } })

    sliced.to_s

    sliced.slice!(2)
    sliced.to_s
