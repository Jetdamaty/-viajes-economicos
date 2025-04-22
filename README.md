import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Menu, MapPin, DollarSign, Lightbulb, Mail, Globe, BookOpen, Map, Languages, SlidersHorizontal } from "lucide-react";

export default function ViajesEconomicos() {
  return (
    <div className="min-h-screen bg-white text-gray-900">
      <header className="p-4 flex justify-between items-center shadow-md">
        <h1 className="text-2xl font-bold">Viajes Económicos</h1>
        <Menu className="w-6 h-6" />
      </header>

      <main className="p-6 grid gap-6">
        <section>
          <h2 className="text-xl font-semibold mb-2">Destinos Recomendados</h2>
          <div className="grid sm:grid-cols-2 lg:grid-cols-3 gap-4">
            <Card>
              <CardContent className="p-4">
                <MapPin className="mb-2" />
                <h3 className="font-bold text-lg">Budapest</h3>
                <p>Una joya europea con termas, historia y precios accesibles.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent className="p-4">
                <MapPin className="mb-2" />
                <h3 className="font-bold text-lg">Ciudad de México</h3>
                <p>Comida deliciosa, cultura vibrante y alojamiento económico.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent className="p-4">
                <MapPin className="mb-2" />
                <h3 className="font-bold text-lg">Lisboa</h3>
                <p>Calles encantadoras, buena gastronomía y opciones muy asequibles.</p>
              </CardContent>
            </Card>
          </div>
        </section>

        <section>
          <h2 className="text-xl font-semibold mb-2">Consejos para Ahorrar</h2>
          <div className="grid sm:grid-cols-2 lg:grid-cols-3 gap-4">
            <Card>
              <CardContent className="p-4">
                <Lightbulb className="mb-2" />
                <h3 className="font-bold text-lg">Vuela entre semana</h3>
                <p>Martes y miércoles suelen ser los días más baratos para volar.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent className="p-4">
                <Lightbulb className="mb-2" />
                <h3 className="font-bold text-lg">Aprovecha el transporte público</h3>
                <p>Evita taxis y apps caras; los abonos de transporte son clave.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent className="p-4">
                <Lightbulb className="mb-2" />
                <h3 className="font-bold text-lg">Reserva con antelación</h3>
                <p>Los vuelos y alojamientos suelen ser más baratos si reservas temprano.</p>
              </CardContent>
            </Card>
          </div>
        </section>

        <section>
          <h2 className="text-xl font-semibold mb-2">Presupuestos por Ciudad</h2>
          <Card>
            <CardContent className="p-4">
              <DollarSign className="mb-2" />
              <p><strong>Lisboa</strong>: Alojamiento desde 25€, menú del día por 10€, atracciones gratuitas con Lisboa Card.</p>
              <p><strong>Bangkok</strong>: Comidas callejeras desde 2€, hostales por 15€, templos gratuitos.</p>
              <p><strong>Praga</strong>: Cerveza barata, paseos por el casco antiguo y alojamiento low-cost.</p>
            </CardContent>
          </Card>
        </section>

        <section>
          <h2 className="text-xl font-semibold mb-2">Blog de Experiencias</h2>
          <div className="grid sm:grid-cols-2 gap-4">
            <Card>
              <CardContent className="p-4">
                <BookOpen className="mb-2" />
                <h3 className="font-bold text-lg">Cómo recorrí Europa con 500€</h3>
                <p>Consejos reales de alojamiento, transporte y comida en 3 semanas de viaje.</p>
              </CardContent>
            </Card>
            <Card>
              <CardContent className="p-4">
                <BookOpen className="mb-2" />
                <h3 className="font-bold text-lg">Mis 5 errores al viajar solo por Asia</h3>
                <p>Errores comunes que puedes evitar si viajas por el Sudeste Asiático.</p>
              </CardContent>
            </Card>
          </div>
        </section>

        <section>
          <h2 className="text-xl font-semibold mb-2">Mapa de Destinos</h2>
          <Card>
            <CardContent className="p-4 text-center">
              <Map className="mx-auto mb-2" />
              <p>Próximamente: mapa interactivo con recomendaciones y rutas.</p>
            </CardContent>
          </Card>
        </section>

        <section>
          <h2 className="text-xl font-semibold mb-2">Multilenguaje</h2>
          <Card>
            <CardContent className="p-4 text-center">
              <Languages className="mx-auto mb-2" />
              <p>Disponible pronto en inglés, español y francés.</p>
            </CardContent>
          </Card>
        </section>

        <section>
          <h2 className="text-xl font-semibold mb-2">Comparador de Precios</h2>
          <Card>
            <CardContent className="p-4 text-center">
              <SlidersHorizontal className="mx-auto mb-2" />
              <p>Herramienta futura para comparar vuelos, alojamientos y actividades.</p>
            </CardContent>
          </Card>
        </section>

        <section className="text-center mt-10">
          <h2 className="text-xl font-semibold mb-2">Contacto</h2>
          <p className="mb-4">¿Tienes dudas o quieres colaborar? Escríbeme:</p>
          <Button className="flex items-center gap-2 mx-auto">
            <Mail className="w-4 h-4" /> Contactar
          </Button>
        </section>
      </main>

      <footer className="p-4 text-center text-sm text-gray-500">
        © 2025 Viajes Económicos. Todos los derechos reservados.
      </footer>
    </div>
  );
}
