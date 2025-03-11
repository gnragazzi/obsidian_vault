Serializar o deserealizar un JSON es la acción de establecer una clase que extienda de `JsonSerializer<T>`, de manera de poder establecer una forma determinada en que un Json leido desde un archivo (o recibido de una BD o a través de internet) parseé la información a un objeto Java.$^1$
***
Ejemplo:
```
import java.io.IOException;

import com.fasterxml.jackson.core.JsonGenerator;
import com.fasterxml.jackson.core.JsonParser;
import com.fasterxml.jackson.core.ObjectCodec;
import com.fasterxml.jackson.databind.DeserializationContext;
import com.fasterxml.jackson.databind.JsonDeserializer;
import com.fasterxml.jackson.databind.JsonNode;
import com.fasterxml.jackson.databind.JsonSerializer;
import com.fasterxml.jackson.databind.SerializerProvider;

import org.springframework.boot.jackson.JsonComponent;

@JsonComponent
public class MyJsonComponent {

	public static class Serializer extends JsonSerializer<MyObject> {

		@Override
		public void serialize(MyObject value, JsonGenerator jgen, SerializerProvider serializers) throws IOException {
			jgen.writeStartObject();
			jgen.writeStringField("name", value.getName());
			jgen.writeNumberField("age", value.getAge());
			jgen.writeEndObject();
		}

	}

	public static class Deserializer extends JsonDeserializer<MyObject> {

		@Override
		public MyObject deserialize(JsonParser jsonParser, DeserializationContext ctxt) throws IOException {
			ObjectCodec codec = jsonParser.getCodec();
			JsonNode tree = codec.readTree(jsonParser);
			String name = tree.get("name").textValue();
			int age = tree.get("age").intValue();
			return new MyObject(name, age);
		}

	}

}
```
***
$^1$. [https://docs.spring.io/spring-boot/reference/features/json.html]
