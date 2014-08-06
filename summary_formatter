class SummaryFormatter
  def initialize(step_mother, io, options)
    @io = io
  end

  def before_feature(feature)
    line = ''
    for i in 0..feature.short_name.size
      line += '_'
    end
    @io.puts feature.short_name
    @io.puts line
    @io.puts
    @io.puts feature.description
    @io.puts
    @io.puts "Scenarios:"
    feature.feature_elements.each do |e|
      @io.puts "  #{e.name}"
    end
    @io.puts
    @io.puts
  end
end
