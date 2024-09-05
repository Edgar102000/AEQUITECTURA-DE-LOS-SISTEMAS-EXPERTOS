Módulo de adquisición de conocimiento

class Expert:
    def __init__(self, name):
        self.name = name
    
    def provide_knowledge(self):
        # El experto provee el conocimiento en forma de reglas
        return {
            'dolor de cabeza': 'toma un analgésico',
            'fiebre': 'toma paracetamol',
            'tos': 'toma un jarabe para la tos'
        }
