/**
 * 
 *
 *
 */
import { Label } from "@/components/ui/label"
import { Textarea } from "@/components/ui/textarea"
import { Button } from "@/components/ui/button"

export default function Component() {
  return (
    <div className="flex flex-col items-center justify-center min-h-[100dvh] bg-gradient-to-br from-rose-200 to-violet-200 px-4 py-12 sm:px-6 lg:px-8">
      <header className="text-center space-y-2">
        <h1 className="text-4xl font-bold text-primary">Para mi amor</h1>
        <img
          src="/placeholder.svg"
          width={400}
          height={400}
          alt="Couple"
          className="mx-auto rounded-full aspect-square object-cover"
        />
      </header>
      <div className="max-w-3xl space-y-8 mt-12">
        <div className="prose text-primary-foreground">
          <h2>Mi querida,</h2>
          <p>
            Cada día que paso a tu lado es un regalo. Tu sonrisa ilumina mi mundo y tu amor me llena el corazón. Eres la
            razón por la que despierto con una sonrisa cada mañana y la última persona en la que pienso antes de dormir.
          </p>
          <p>
            Quiero que sepas cuánto te amo y lo afortunado que me siento de tenerte en mi vida. Eres mi mejor amiga, mi
            confidente y mi compañera de vida. Juntos, podemos enfrentar cualquier cosa que se nos presente.
          </p>
          <p>
            Gracias por ser tú, por aceptarme tal y como soy y por acompañarme en este viaje llamado vida. Te amo con
            todo mi corazón.
          </p>
          <p>Tuyo por siempre,</p>
          <p className="font-bold">[Tu nombre]</p>
        </div>
        <div className="grid grid-cols-2 gap-4">
          <img src="/placeholder.svg" width={300} height={300} alt="Couple 1" className="rounded-lg object-cover" />
          <img src="/placeholder.svg" width={300} height={300} alt="Couple 2" className="rounded-lg object-cover" />
        </div>
      </div>
      <div className="max-w-md w-full mt-12">
        <form className="space-y-4">
          <div>
            <Label htmlFor="message">Déjame un mensaje</Label>
            <Textarea id="message" name="message" placeholder="Escribe tu mensaje aquí..." className="w-full" />
          </div>
          <Button type="submit" className="w-full">
            Enviar
          </Button>
        </form>
      </div>
    </div>
  )
}
